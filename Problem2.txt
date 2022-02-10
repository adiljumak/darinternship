
function plant(seed, water, fert, temp) {
  var ans = ""
  for(let i = 0; i < water; i += 1) {
    ans += '-'.repeat(water);
    ans += seed.repeat(fert);
  }
  if(temp >= 20 && temp <= 30) {
    return ans;
  }
  return ('-'.repeat(ans.length - 1) + seed)
}





console.log(plant("@", 3, 3, 25));
console.log(plant("&", 5, 1, 20));
console.log(plant("§", 3, 3, 15));



