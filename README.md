# opa-eval-xperiment
Experiment to mimic opa playground

Here are the tests I ran

1. `opa eval --input input.json  --data test.rego "data.hello"`  results in `{}`
2. `opa eval --input input.json  --data test.rego "hello"` results in `rego_unsafe_var_error`
3. `opa eval --input input.json  --data test.rego "play.hello"` results in `rego_unsafe_var_error`

But if you 

1. Go to playground - https://play.openpolicyagent.org/p/ACpt6leoEx which has same input & rego files, 
2. Select word "hello" on line 21
3. Click on "Evaluate Selection" in top right corner
4. You will see valid text in output panel
