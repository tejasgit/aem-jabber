Custom CLient context  session store which processes a JSON object does not display all the values 

			I have created a new session store which reads data from the JSON file and displays the information in the client context. However, when I try to create segments based on the store properties, the generic store property window does not show the nested elements of the JSON. Here is the description

		

			The JSON Structure and the list of properties are given below. Column1 shows the JSON structure and Column2 displays the list of elements that I see when I drag a generic store property and select the cusom store. While the arrays is something that I can manage using the contains feature by checking


			if(prop1) contains val1 display teaser1

			However, the nested values like live_videoid , timestamp etc are something that I cant fetch in the store. Refer to attached screenshot and package for more info
			
			Package - https://github.com/tejasgit/aem-jabber/blob/master/customstore-1.0-SNAPSHOT.zip
			Segment Screenshot - https://github.com/tejasgit/aem-jabber/blob/master/segment.png

		
					JSON Structure
					
						{  
						   "name":"In-A-Gadda-Da-Leela",
						   "description":"Son, as your lawyer, I declare y'all are in a 12-piece bucket o' trouble. But I done struck you a deal: Five hours of community service cleanin' up that ol' mess you caused.",
						   "live":{  
						      "live_videoID":"1524",
						      "live_timestamp_start":1433181600,
						      "live_timestamp_end":1446487200
						   },
						   "archived":{  
						      "videoID":"yBevB7XFcA0e9wC0q7niuA"
						   },
						   "products":[  
						      "Cloud", "Chatter"
						   ],
						   "tags":[  
						      "SMB", "Enterprise"
						   ],
						   "speakers":[  
						      {  
						         "speaker_name":"Test User 1",
						         "speaker_title":"Chair, President", "image":"WtxrUJ_I.png"
						      },
						      {  
						         "speaker_name":"Test User 2",
						         "speaker_title":"CEO of Company","image":"7FsEghTJ_400x400.jpeg"
						      },
						      {  
						         "speaker_name":"Test User 3",
						         "speaker_title":"Co-Founder of Company","image":"gFVwu2oG.jpeg"
						      }
						   ]
						}

				List of properties seen on Generic Store
				
						name
						description
						live
						archived
						products
						tags
						speakers
