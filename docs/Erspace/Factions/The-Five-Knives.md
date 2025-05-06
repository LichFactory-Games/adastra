```dataview
>> TABLE WITHOUT ID
>> embed(art) AS "Art",
>>     "<span style='display: block; border-bottom: 2px solid var(--text-accent); text-align: center; margin-bottom: 5px;'>" + link(file.link, Title) + "</span>" AS Title,
>>	(":rif_heart: ") + condition AS "Condition", 
>>	(":fas_globe_americas: ") + link(location, location) AS "Location"  
>> WHERE type = "npc" AND faction = "The Five Knives"
>> SORT file.name desc
>>```