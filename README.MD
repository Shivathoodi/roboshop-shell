
#!/bin/bash

username="newuser"


if id "$username" &>/dev/null;
then
    echo "User $username already exists."
else
    # Add the user
    useradd "$username"
    echo "User $username added."
fi