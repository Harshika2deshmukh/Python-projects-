class Contact:
    def __init__(self, name, phone, email):
        self.name = name
        self.phone = phone
        self.email = email

    def display(self):
        print(f"Name: {self.name}")
        print(f"Phone: {self.phone}")
        print(f"Email: {self.email}")
        print("-------------------")


contacts = []

def add_contact():
    name = input("Enter Name: ")
    phone = input("Enter Phone: ")
    email = input("Enter Email: ")
    contact = Contact(name, phone, email)
    contacts.append(contact)
    print("Contact Added Successfully!\n")


def view_contacts():
    if not contacts:
        print("No contacts available.\n")
    else:
        for contact in contacts:
            contact.display()


def search_contact():
    name = input("Enter Name to Search: ")
    found = False
    for contact in contacts:
        if contact.name.lower() == name.lower():
            contact.display()
            found = True
            break
    if not found:
        print("Contact Not Found.\n")


def update_contact():
    name = input("Enter Name to Update: ")
    for contact in contacts:
        if contact.name.lower() == name.lower():
            contact.phone = input("Enter New Phone: ")
            contact.email = input("Enter New Email: ")
            print("Contact Updated Successfully!\n")
            return
    print("Contact Not Found.\n")


def delete_contact():
    name = input("Enter Name to Delete: ")
    for contact in contacts:
        if contact.name.lower() == name.lower():
            contacts.remove(contact)
            print("Contact Deleted Successfully!\n")
            return
    print("Contact Not Found.\n")


# Main Menu
while True:
    print("---- CONTACT LIST MENU ----")
    print("1. Add Contact")
    print("2. View Contacts")
    print("3. Search Contact")
    print("4. Update Contact")
    print("5. Delete Contact")
    print("6. Exit")

    choice = input("Enter choice: ")

    if choice == "1":
        add_contact()
    elif choice == "2":
        view_contacts()
    elif choice == "3":
        search_contact()
    elif choice == "4":
        update_contact()
    elif choice == "5":
        delete_contact()
    elif choice == "6":
        print("Exiting Program...")
        break
    else:
        print("Invalid Choice! Try Again.\n")
