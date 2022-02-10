
function color_pattern_times(cols) {
  var ans = 0;
  if(Object.keys(cols).length > 0) {
    ans += 2;
  } 
  for(let i = 1; i < Object.keys(cols).length; i += 1) {
    if(cols[i] !== cols[i - 1]) {
      ans += 1;
    }
    ans += 2;
  }
  return ans;
}



var cols1 = ['Red', 'Blue', 'Red', 'Blue', 'Red'];
var cols2 = ['Blue'];
var cols3 = ["Red", "Yellow", "Green", "Blue"];
var cols4 = ["Blue", "Blue", "Blue", "Red", "Red", "Red"];

console.log(color_pattern_times(cols4));

