//Password Validator
//Got to have one uppercase character
//Got to have one lowerCase character
//Minimum 8 Characters long
//And got to have one special charater

function isPasswordValid(input) {
  if (
    hasUpperCase(input) &&
    hasLowerCase(input) &&
    hasMinimumCharacter(input) &&
    hasSpecialCharacters(input)
  ) {
    console.log(`Password is valid`);
  }

  if (!hasUpperCase(input)) {
    console.log(`Password needs a capital letter`);
  }

  if (!hasLowerCase(input)) {
    console.log("Password needs a lowecase letter");
  }
  if (!hasMinimumCharacter(input)) {
    console.log(`Password has to be minimum 8 characters long`);
  }
  if (!hasSpecialCharacters(input)) {
    console.log(`Password needs a special character`);
  }
}

//Special Characters
function hasSpecialCharacters(input) {
  let specialCharacters = ["@", "#", "$", "%", "^", "&", "*", "!"];
  for (let i = 0; i < input.length; i++) {
    for (let j = 0; j < specialCharacters.length; j++) {
      if (input[i] === specialCharacters[j]) {
        return `${specialCharacters[i]} is found`;
      }
    }
  }
}

//Has uppserCase
function hasUpperCase(input) {
  //loop through the input to check
  for (let i = 0; i < input.length; i++) {
    //check every character
    if (input[i] === input[i].toUpperCase() && typeof input !== "number") {
      return true;
    }
  }
}

//Has lowerCase
function hasLowerCase(input) {
  //loop through the input to check
  for (let i = 0; i < input.length; i++) {
    //check every character
    if (input[i] === input[i].toLowerCase()) {
      return true;
    }
  }
}

//Has minimum 8 characters
function hasMinimumCharacter(input) {
  //No loop necessary
  if (input.length >= 8) {
    return true;
  }
}
isPasswordValid("%passWord");
