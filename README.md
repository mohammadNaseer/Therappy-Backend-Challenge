## Tools
Built With the Following Technologies/Tools:
- Node.js (Express)

Text Editor:
- VSCode

## Development

### To run an instance of this app locally

- install needed dependencies
- install express (npm install --save)
- install ejs (npm install ejs)
- run server.js from terminal using (node server)
- you may need to refresh the page once AFTER it loads


(testcase)

######case 1######
#input
http://localhost:8080

#output
404 - NOT Found

######case 2######
#input
http://localhost:8080/I/want/title?address=google.com

#output
Following are the titles of given websites:
. google.com - "Google"

######case 3######
#input
http://localhost:8080/I/want/title?address=http://yahoo.com

#output
Following are the titles of given websites:
. https://yahoo.com - Title Tag missing

######case 4######
#input
http://localhost:8080/I/want/title?address=google.com&address=dawn.com/events/

#output
Following are the titles of given websites:
. google.com - "Google"
. www.dawn.com/events/ - "Events - DAWN.COM - DAWN.COM"

######case 5######
#input
http://localhost:8080/I/want/title?address=asdasdasd

#output
. asdasdasd - NO RESPONSE             