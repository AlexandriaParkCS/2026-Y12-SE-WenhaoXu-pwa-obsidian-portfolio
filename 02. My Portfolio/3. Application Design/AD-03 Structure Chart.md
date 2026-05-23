***Dashboard Generation***
The Dashboard Generation process is responsible for producing a personalised list of chores in the application. This process is initiated when a user requests to view their dashboard, typically after logging in.

![[Pasted image 20260521130635.png]]
At the top of the hierarchy is the generate dashboard module, which coordinates all the submodules to retrieve the user data, process and then display the relevant data regarding the chores to the user. The tasks are delegated to two key data modules, the Get User Data and the Get Chores modules. These modules will access the SQL database to retrieve the user's profile and the list of chores respectively. 

Once the data is retrieved, the data is used by the Get Chores/Get list of chores, which matches the user_id to the foreign key in the chores database for displaying. Similarly, the chores that are given are automatically sorted by the time.

Then, the chores are displayed on the dashboard sorted by time.

Algorithm:

BEGIN GenerateDashboard  
	UserSummary = GetUserData(UserID)  
	ChoreSummary = GetChores(UserID)  
  
DISPLAY UserSummary  
  
IF ChoreSummary is empty  
	DISPLAY "No chores scheduled yet!"  
ELSE  
	DISPLAY ChoreSummary  
ENDIF  
  
END

BEGIN GetChores  
  
	ChoreQuery = SELECT Chores for UserID  
	Chores = RetrieveChores(ChoreQuery)  
  
	CategorisedChores = CategoriseByWeekday(Chores)  
  
	SummaryRow = 0  
  
	FOR Weekday in CategorisedChores  
  
		ChoreSummary[SummaryRow] = Weekday  
  
		NEXT SummaryRow  
  
		FOR Chore in Weekday  
  
			ChoreSummary[SummaryRow] = Chore  
  
			NEXT SummaryRow  
  
		ENDFOR  
  
	ENDFOR  
  
	RETURN ChoreSummary  
  
END
