# FahrradKiel

## Deployment with database and API

## Development

### System Requirements

 - Node (Latest Version)
 - PHP > 7.1.3
 - PostgreSQL 
 - Postgis extension for postgresql
 - Composer ( Latest version ) 

### installation
Clone repository
```
git clone https://github.com/SanaGhaffar/FahrradTour.git
```
### REST Api - installation and config

Install PHP dependencies
```
cd apps/ctapi
composer install
```
To configure api settings open below file and change database connection
```
apps/ctapi/.env
```

Now run below command from current folder location
```
php -S 127.0.0.1:8080 -t public public/index.php
```

#### Application frontend - installation and config
Install node dependency 
```
cd apps/ctweb
npm install
```

To change API_URI, edit below file
```
apps/ctweb/src/helpers/ctKielApi.js
```
Now run below command
```
cd apps/ctweb
npm start
```

note: Default config

 - Development Server URL: http://localhost:3000
 - Api URL: http://127.0.0.1:8080/ 
