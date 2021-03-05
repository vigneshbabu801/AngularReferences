# AngularReferences
Blob File Insert - ORACLE

 

https://github.com/oracle/node-oracledb/blob/master/examples/lobinsert1.js

 

File Upload - Angular

 

https://stackoverflow.com/questions/47936183/angular-file-upload

 

Download File in Node JS Sent from NG

 

  filename = req.body.file;

  let receiveSuccessUpload = [];

  let receivedFile = req.file.buffer

  console.log(req.file.mimetype);

  console.log(req.file.originalname);

  fs.writeFile(req.file.originalname,req.file.buffer,function (err){

    if(err){

      throw err;

    }

  })
  
  -----------------------------------------------------------------------------------------------------------
  
  Install Pm2 Globally 


	
npm install pm2 -g


Start the Servers


	
Go to the folders respectively
	Run pm2 start index.js --watch


Startup  Script


	
Once Started all applications, save the list which need to respawn
	Run pm2 save
	After rebooting the server, brings back previously saved processes (via pm2 save)
	

		
Run pm2 resurrect
	
	
	Pm2 kill
  
  --------------------------------------------------------------------------------------------------------
  
  Import-Module SimplySql

Open-OracleConnection -ConnectionName test -DataSource  silddb5035.ftdc.cummins.com -Port 1527 -ServiceName rbautod1

$query = "select * from user_details"

Invoke-SqlQuery -Query $query -ConnectionName test

 

Close-SqlConnection -ConnectionName test
