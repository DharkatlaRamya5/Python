import random
import string
adjectives=["mango","guava","apple","banana"]
nouns["ramya","siri","ammu","akshu","laddu"]
def generate_username(include_number=True,include_special=False):
  adj=random.choice(adjectives)
  noun=random.choice(nouns)
  username=adj+noun
  if include_number:
      username+=str(random.radiant(10.99))
  if include_special:
      username+=random.choice("!@#$%^&*")
      reurn username
def get_user_preferences():
  add_number=input("includea number?(yes/no):").strip().lower()=="yes"
  add_special=inpu("include a special character?(yes/no):").strip().lower()=="yes"
  return add_number,add_special
def save_to_file(username):
  with open ("username.txt","a")as file:
    file.write(username+"\n")
print(f"username'{username}'saved successfully!")
def main():
  print("welcome to the username generator!")
  while True:
    add_number,add_special=get_user_peferences()
    username=generate_username(add_number,add_special)
      print(f"generated username:{username}")
      save=input("do ypu want to save this username ?(yes/no):").strip().lower()
      if save=="yes"
          save_to_file(username)
          again=inout("generate another username?(yes/no:").strip().lower.()
          if again!="yes"
            print("thanks for using username generator!")
            beak
if_name_=="_main_":
  main()
      
    

