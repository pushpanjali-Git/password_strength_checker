# password_strength_checker
password strength checker
def strong_password(Password):#check password strength - strong or weak
 if len(Password)<8:
   return false
 if not any(char.isdigit() for char in Password):
   return false
 if not any(char.islower() for char in password):
   return false
 if not any(char.isupper() for char in password):
   return false
 if not any(char in '!@#%^&*()_+' for char in password):
   return false
 return true

 #calling the function
 print(strong_password('Pushpa1122'))
 print(strong_password("stronggit"))
 
 

