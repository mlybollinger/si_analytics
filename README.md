# si_analytics

This repository stores the scripts I used to test the functionality of Salesforce's BLIP model to generate alt-text for Smithsonian images. I was assigned to test whether the image captions generated by BLIP could feasibly serve as alt-text to be read out by browsers on Smithsonian web properties. To do this, I used Twitter's API to gather images from all Smithsonian Twitter accounts, then had BLIP generate captions for a representative sample of them. I tested the captions both by evaluating them manually and by using BLIP's own Image-Text Matching score. I then plugged the resulting data into an interactive dashboard created with Plotly and Dash. 

TwitterAPISearch.ipynb contains the code I used to query Twitter's API and extract the images. The subsequent tests I performed can be found in BLIP_caption_scoring.ipynb. And the dashboard I built in si_data_visualization.ipynb uses the data in an interactive visualization the user can manipulate through radio buttons.
