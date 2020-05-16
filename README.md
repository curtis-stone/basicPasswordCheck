# basicPasswordCheck
Basic JavaScript password check function

    function isValidPassword(password) {
        if (password.includes('password')) {
            return false // if string entered includes 'password' it is invalid
        }
        else if (password.length >= 5) {
            return true // password is only valid if it's length is at least 5 characters
        }
        else {return false}
    }

    //try it out below

     console.log(isValidPassword('asdfp')) // returns true (at least 5 characters)
     console.log(isValidPassword('abc123!@#$')) // returns true (at least 5 characters)
     console.log(isValidPassword('asdfpeveepassword')) // returns false since it has the string 'password in it'
