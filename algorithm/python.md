## Creating session with requests module
Useful where you need to use session information to access the page which requires authentication.
```python
import requests

url = 'https://mypage.com/login'
form_data = {'username':'' , 'password':''}
s = requests.Session()
s.post(url,form_data)
```
For form data, submit the page (login) in the browser and check in the network tab about what data is being submitted. use the same. 

After this, use session object for any get/post calls.