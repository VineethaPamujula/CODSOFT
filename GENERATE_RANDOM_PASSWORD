from tkinter import *
import string
import random
root = Tk()
Tk.config(root, bg="pink")
root.title("password generator")
root.geometry("450x300+500+200")
root.resizable(False,False)
length=Label(root,text="Enter the length of your password:",font=("arial",15))
length.grid(row=10, column=20,padx=5,pady=5)
data = IntVar()
text=Entry(root, textvariable=data,font=("arial",20))
text.grid(row=12, column=20,padx=5,pady=5)
def buttonFunction():
     letters = string.ascii_letters
     numbers = string.digits
     special_characters = string.punctuation
     a = letters + numbers + special_characters
     pwd = ""
     for i in range(data.get()):
         pwd += random.choice(a)
     emptylabel.config(text="your password is : " + str(pwd),font=("arial",20))
b=Button(root,text="generate",command=buttonFunction,font=("arial",15))
b.grid(row=14, column=20,padx=5,pady=5)
emptylabel=Label(root,fg="black")
emptylabel.grid(row=16,column=20)
root.mainloop()

