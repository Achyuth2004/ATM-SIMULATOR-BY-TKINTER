from tkinter import *
from tkinter import messagebox

root = Tk()
root.title('ATM SIMULATOR')
root.configure(bg='blue')
root.geometry('800x500')
root.resizable(0, 0)  # This prevents window resizing

# User details
user_pin = "1523"  # Convert PIN to a string
user_balance = 97432.50
user_name = "Mr. ACHYUTH"

input_pin = StringVar()

def verify(input_pin):
    if input_pin == user_pin:
        messagebox.showinfo("Verification", "Password Verified")
    else:
        messagebox.showerror("Verification", "Incorrect Password")
        withdraw.destroy()
        

def withdraw():
    new_window = Toplevel(root)
    new_window.geometry('800x500')

    label1 = Label(new_window, text='Enter 4 DIGIT PIN : ', font=('Arial', 18))
    label1.grid(row=0, column=0)

    entry1 = Entry(new_window, textvariable=input_pin)  # Use textvariable to get the PIN
    entry1.grid(row=0, column=1)

    button = Button(new_window, text="Submit", command=lambda: verify(entry1.get()))
    button.grid(row=1, column=1)

# Main label
label = Label(root, text="              ****SBI****              ", font=("Arial", 20))
label.place(relx=0.4, rely=0.1, anchor=CENTER)

# Withdraw button
button = Button(root, text="Withdraw", font=('arial', 18, 'italic'), fg='orange', bg='black', relief=RAISED, bd=15, command=withdraw)
button.place(relx=0.2, rely=0.2)

# Deposit button
button = Button(root, text="Deposit", font=('arial', 18, 'italic'), fg='orange', bg='black', relief=RAISED, bd=15)
button.place(relx=0.5, rely=0.2)

# Check balance button
button = Button(root, text="Check Balance", font=('arial', 18, 'italic'), fg='orange', bg='black', relief=RAISED, bd=15)
button.place(relx=0.5, rely=0.4)

# Deposit button
button = Button(root, text="Deposit", font=('arial', 18, 'italic'), fg='orange', bg='black', relief=RAISED, bd=15)
button.place(relx=0.2, rely=0.4)

# Change PIN button
button = Button(root, text="Change PIN", font=('arial', 18, 'italic'), fg='orange', bg='black', relief=RAISED, bd=15)
button.place(relx=0.2, rely=0.6)

# Exit button
button = Button(root, text="EXIT", font=('arial', 18, 'italic'), fg='orange', bg='black', relief=RAISED, bd=15)
button.place(relx=0.5, rely=0.6)

root.mainloop()
