# Get user input for age and citizenship
age = int(input("Enter your age: "))
citizenship = int(input("Are you a citizen of the country? (1 for yes, 0 for no): "))

# Check if the person is eligible to vote
if age >= 18 and citizenship == 1:
    print("You are eligible to vote!")
    vote = int(input("Do you want to cast your vote? (1 for yes, 0 for no): "))
    if vote == 1:
        party = int(input("Which party do you want to vote for? (1 for BJP, 2 for Congress): "))
        if party == 1:
            print("You have cast your vote for BJP!")
        elif party == 2:
            print("You have cast your vote for Congress!")
        else:
            print("Invalid party choice. Please choose 1 for BJP or 2 for Congress.")
    else:
        print("You have chosen not to cast your vote.")
else:
    print("You are not eligible to vote.")
