# stream-lit
Aouthor-usman
<br>
Import streamlit as st

def login_page():
    st.title("Login Page")
    username = st.text_input("Username")
    password = st.text_input("Password", type="password")

    if st.button("Login"):
        # Yeh sirf example hai, real application mein aapko database se credentials verify karne honge
        if username == "admin" and password == "password":
            st.success("Login successful!")
            # Login successful hone ke baad aap apne application ke main page ko dikha sakte hain
            main_page()
        else:
            st.error("Invalid username or password")

def main_page():
    st.title("Main Page")
    st.write("Welcome to the main page!")

if __name__ == "__main__":
    login_page()
``