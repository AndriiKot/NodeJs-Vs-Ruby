﻿Ruby vs Node.js
ARGV
Creation ARGV
Ruby
arg = ARGV
p arg      # []
Nodejs
let arg = process.argv
console.log(arg)          // ['C:\\Program Files\\nodejs\\node.exe','C:\\Project\\NODE\\RubyVsNodeJs\\app']
Get one argv
Ruby
ruby app.rb one 2 3 hi!
p ARGV[0]             # "one"
ruby app one 2 3 hi!   # not valid ... -- app (LoadError)
Nodejs
node app.js one 2 3 hi!  
or

node app one 2 3 hi!             // valid
console.log(process.argv[2])  // one 
Operator if
Ruby
a,b = ARGV[0],ARGV[1]
ruby app.rb 1 2
p (if a > b then  a else b end)   # "2"
or

p a > b ? a : b     # "2"