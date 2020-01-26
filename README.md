# Decompress-Run-Length-Encoded-List
LeetCode Challenge - Javascript

nums = [1,2,3,4]

var decompressRLElist = function(nums) {
  let output = []
  let increment = 2
  for (let i = 0, i < nums.length, i++) {
    const [freq, val] = nums.slice(i, i + increment) 
    const encode = new Array(freq).fill(val)
    output.concat(encode)
};
