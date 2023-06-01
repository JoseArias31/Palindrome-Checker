# Palindrome-Checker

function palindrome(str) {
  let lowerCase = str.toLowerCase();
  let removeSpecialCharacters = lowerCase.replace(/[_\-.,/)(\s]/g, '')
let reverseTheString = removeSpecialCharacters.split('').reverse().join('');

console.log(reverseTheString)
 if (removeSpecialCharacters === reverseTheString) {
  return true;
 }
 else{
   return false
 }
} 

console.log(palindrome("0_0 (: /-\ :) 0-0"));
