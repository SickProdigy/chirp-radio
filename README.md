This will be a backup of my progress with chirp and programming radios. 

I did end up paying [RadioReference.com](https://www.radioreference.com/) $15.00 to query their database easily. I'll provide that also. I only queried my local results. May query a bit further to take a backup. Don't like how a lot of these sites want monthly bucks when information should be free really. Take a donation at most. The equipment alone is fortune to some. Whatever, over that rant. 

So first I downloaded the [default image](./Kenwood_TK-862G_20251027-default.img) on my radio kenwood tk-862g-1. I bought this for TARPN but it's a 450MHz-490MHz which is business version I shouldn't have bought and got confused somehow. The site was a bit misleading because this model kenwood can be in 420MHz-449MHz or 450MHz-490MHz. Site said this one should be the lower. I thought it needed the number listed in the ebay ad too, so I need to pay more attention on my part. I will be ordering a tk-76x for VHF purposes. Will keep this one around for UHF. May possibly try some soldering to it to get it to meet lower range of the 70cm band, or just buy the proper one..  
Another thing with these kenwood tk-862g-1 UHF in 450MHz-490MHz range, can only receive FM. No DMR (Digital). Need a better radio for that. So looking into some cheaper handhelds to achieve this. A lot of transmissions are done digitally around me so this kind of sucks having an FM only radio. Can pickup a few radio stations when a heli is around, hospitals, and local businesses producing in FM or FMN as shown on [RadioReference](https://www.radioreference.com/db/browse/coid/1). Not that fun to listen to. 

You can see examples for a Query Result for RadioReference below. 
[QueryResult-radioreference.com-chirp-example-NC-Wake-County.csv](QueryResult-radioreference.com-chirp-example-NC-Wake-County.csv) 
[QueryResult-radioreference.com-chirp-example-NC-Wake-County.xlsx](QueryResult-radioreference.com-chirp-example-NC-Wake-County.xlsx)

Which should basically correlate like so from here:
https://www.radioreference.com/db/browse/ctid/1978#cid-4811

From radioreference db you will see something like
`461.9875	WQOL325 	RM 	100.0 PL 	DH Hill Library 	DH Hill Library 	FMN 	Schools`
which in the query result translates to
`61	DH Hill Library	461.9875	split	466.9875	TSQL	100	100	023	NN	023	Tone->Tone	NFM	5		50W	DH Hill Library`	

What was nice is, i could copy the query result and just paste into my radios channel. Working. Pure love when you get your first transmision.

So what I'm told is you have to figure out how chirp labels things vs terms everyone would else would us. 100.0 PL will be TSQL 100.0 and so on. 

I think I will download some default images for other radios and examples in chirp since chirp uses such weird terms vs everyone else. Try to provide as much information I can through git. 

Thanks for your time.

Sick Prodigy / Aaron