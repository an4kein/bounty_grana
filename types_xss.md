⚡️XSS Tips for Beginners: ⚡️

XSS being the most common attack vector in majority of the web applications across pentesting and bug bounty programs, I would like to share some quick handy tips to find them👇

Reflected XSS: ✅

Crawl Application URLs by Active and Passive ways.
Grep = from all urls, Sort -u all duplicates, Pass special characters as value in all the urls and see reflection via kxss.

Manually Try to craft the payload and get XSS. Use Url encoding, base64, Html encoding.

Stored XSS: ✅

Crawl application pre and post login, Check forms where you can submit data which can be stored like profile etc.

Blind XSS: ✅

Check sections like comments, feedbacks, support tickets.
These can be used to check Blind XSS too.

DOM XSS: ✅

Crawl all js files from the target, grep and check most commonly vulnerable sources and sink.

Setup DOM Invader and validate if the input is not sanitized when coming out of sink.

Post Based XSS: ✅

Check Post forms and try to inject special characters in the post forms hidden inputs in body. Validate if they are not sanitized, Inject Payload and craft a post based XSS
