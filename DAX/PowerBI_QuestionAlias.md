Result = 
IF( AND([no_of_days_pending]>=100,[no_of_days_pending]<200),
	150, 
	IF( AND([no_of_days_pending]>=200,[no_of_days_pending]<300),
		250,
		IF( AND([no_of_days_pending]>=300, [no_of_days_pending]<400),
			350, 
			IF( AND([no_of_days_pending]>=400, [no_of_days_pending]<500),
				450,
				IF([no_of_days_pending]>=500,
					600, 
					BLANK()
				)
			)
		)
	)
)