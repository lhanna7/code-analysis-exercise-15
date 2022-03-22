# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident that you know how the function works.
* Write a summary of what the function does.

```js
function (person, petName){
  for (let dog of person.dogs){
    if (dog.name === petName){
      return dog
    }
  }
}
```

Inputs and outputs should be valid JavaScript values!

| Input | Output |
| ----- | ------ |
|  const lauren = {name: "Lauren", dogs: [{name: "Churro", breed: "Border Collie", gender: "Male"}]  }  function (lauren, "Churro")   |   {name: "Churro", breed: "Border Collie", gender: "Male"}    | 
|  const lauren = {name: "Lauren", dogs: [{name: "Percy", breed: "Is Actually a Cat", gender: "Male"}]  }  function (lauren, "Perceus")    |  undefined      | 
|                    |        | 

<table>
  <tr>
    <th>What does this program do?</th>
    <td>This function takes an object (person) and searches the nested object within (dogs) to see if the petName comes up with a match. My assumption is that .dogs is made up of several different properties (name, breed, gender, etc). If the petName parameter pulls a match within that array, then dog will be returned. This function works similarly to .find. If there is not a match (or you use the pets full name instead like I did), it will return as undefined. </td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible
