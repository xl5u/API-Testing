# API-Testing
Welcome everyone and thank you for showing up for my presentation.  Today, I would like to demonstrate how we use Apttus contract management system to support the agreement management system of ABC company.

ABC company has three types of agreements with customers who purchases products and customer support
Non disclosure Agreement (NDA)- unilateral
Non disclosure Agreement - bilateral
And Service level agreement (SLA)
We configured three flows for the three types of agreement and in the next 15 min I will demo each of them.  Along the flows, I will also show you some of the cool features we configured for ABC company.
Now Let me switch to SF

The first flow I will demo is NDA -unilateral.  First, I went to ABC company's account page and created a NDA unilateral agreement - 
All NDA are in English
We configure the process that When NDA unilateral is selected, the agreement is generated automatically in PDF and sent via email to the Primary Contact. The template used is NDA unilateral template.

When Bilateral is selected, the agreement is forwarded to the Legal Queue for review. 
SLA
Wizard generates user-friendly on-screen Wizards to quickly create contracts. The Wizards are intended for use by non-expert users - it prompts the end user to answer a series of on-screen questions then creates the Agreement record. It removes unnecessary fields from the creation steps that might confuse the users and simplify the flow, saving the time for end users

I use wizard to create my SLA agreement, and then I will add some line items to the agreement. I save it and now the agreement is ready for generating the contract.   We configure a query template for the generation step to dynamically pick template depends on the language and region on the agreement.  You can also see two buttons "Submit" and "Generate" here.  If you have an very complex template with lots of condition logics and clause, it might take long time to generate the document. What submit button does is allow user to submit a batch job of contract generating to run in background.  For the demo, I will just use generate.  Now let's look at the generated contract to see if everything is correct.
I open the generated document and see that account name, start, end dates and term are there.  The support exhibits also dynamically determines what support customer gets.  Same for the clauses in terms and conditions, which is determined by the support exhibits and region and agreement category.  Now everything looks ok, now I can send it to Diego for review. Now I am diego, I open the document in my email, I don't like the end date and term, so I changed them, and edit the governing law a bit.  And send it back.  Now I am myself and open the document diego sent me and I first check it in to save a copy of what diego's changes.  I checked it out and I agree with diego so I check in with reconcile.  Now I also want to get a final version of this, so I check in again with final selected, we edit the system properties that allow automatically generated PDF when final is checked.  Now I am back to SF and look at the document version.  PDF is here and it is ready for signature.  I send it to diego for signature.  Diego acts quickly and replies with a signed PDF document.  So I upload the signed PDF document here and the agreement is ready for activation.  That's the end to end flow of SLA.  Since the CEO is concerned about the time spend waiting for customer signature, I create a report to see th cycle time of status chnaged from other party signature to fully signed.  This is the report.  You can see the average time 
