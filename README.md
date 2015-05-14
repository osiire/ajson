# ajson
The Specification of algebraic JSON

```
(* OCaml *)
type json = 
  | Object of (string * json) list
  | Bool of bool
  | Number of float
  | Int of int
  | String of string
  | List of json list
  | Null
  | Union of string * json
```

example.

   {
     "Card": "Joker" {}
   }

   {
     "Card": "Number" 1
   }