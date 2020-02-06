## Web developer ##
### Resume ###

<img align="right" width="100" height="100" src="\Images\Me.jpg" alt="me">

1. #### Personal details ####
**Name              :** Viachaslau Shabaltsiyeu
**E-mail            :** enliven001@mail.ru
**Telephone Number  :** +375 (29) 253-02-96
**GitHub            :** [my GitHub](https://github.com/enl001)

-------------------------------------------------------------
2. #### Objective & Summary ####

Start a career as a web developer in EPAM Systems and in 5 years become an Engineering Lead/ Team Lead.

- Five years of special software and embedded systems software development experience
- Proficient in an assortment of languages and technologies, including C#/C++, JavaScript, TypeScript, SQL,  ASP.Net, Angular
- I have good analytical skills and experience in conducting scientific research

##### Hobby #####

- Mountain hiking
- Photography

---------------------------------------------------------------
3. #### Skills ####

- **C#**         ++
- **Asp.Net**    +
- **HTML5**      +
- **CSS3**       +
- **JavaScript** +
- **TypeScript** +
- **Angular 2+** +
- **Agile**      +
- **Git**        +

-----------------------------------------------------------------
4. #### Experience ####

- "Object-Oriented Programming Fundamentals in C#" course
- "Building a Web App with ASP.NET Core, MVC, Entity Framework Core, Bootstrap, and Angular" course
- "LINQ Fundamentals" course
- [Codewars](https://www.codewars.com/users/enl001)

> [Codewars "Strings Mix"](https://www.codewars.com/kata/5629db57620258aa9d000014) 

````
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text.RegularExpressions;

public class Mixing 
{
  public static string Mix(string s1, string s2)
  {
    s1 = Regex.Replace(s1, "[^a-z]", "");
    s2 = Regex.Replace(s2, "[^a-z]", "");
    var s1Unic = s1.Distinct().OrderBy(c => c);
    var s2Unic = s2.Distinct().OrderBy(c => c);
    var merge = s1Unic.Concat(s2Unic).Distinct().OrderBy(c => c);
    var sCountChar = new List<string>();
      
    foreach (var c in merge)
    {
      var count1 = s1.Where(s => s == c).Count();
      var count2 = s2.Where(s => s == c).Count();

      if (count1 <= 1 && count2 <= 1) continue;
      if (count1 > count2) sCountChar.Add($"1:{count1}{string.Concat(Enumerable.Repeat(c,count1))}");
      if (count1 < count2) sCountChar.Add($"2:{count2}{string.Concat(Enumerable.Repeat(c, count2))}");
      if (count1 == count2) sCountChar.Add($"3:{count1}{string.Concat(Enumerable.Repeat(c, count1))}");
    }
    sCountChar = sCountChar.OrderByDescending(s => s.Substring(2, 1))
                           .ThenBy(c => c.Substring(0, 1)).ToList();

    var result = new List<string>();
    foreach (var item in sCountChar)
    {
      var r = item;
      r = r.Replace("3", "=");
      result.Add(r.Remove(2, 1));
    }
    return string.Join("/",result);
  }
}
````
> [Codewars "Sort the odd"](https://www.codewars.com/kata/578aa45ee9fd15ff4600090d)
````
function sortArray(array) {
  let odd = [];
  for(const n of array)
  {
    if(n%2!==0) odd.push(n);
  }
  odd.sort((a,b)=>{return a-b});
  let k=0;
  for(let i= 0; i< array.length; i++)
  {
    if(array[i]%2!==0) {array[i]=odd[k]; k++;}
  }
  return array;
}
````

##### Working experience #####

- 2014 - Present  : Researcher
- 2012 - 2014     : Junior Researcher

##### Other skills #####

- Experienced in such software package as MATLAB.

-----------------------------------------------------------------
5. #### Education ####

- 2012  Researcher. Military Academy of the Republic of Belarus
- 2009  Master of Engineering. Military Academy of the Republic of Belarus
- 2008  Engineer. Telecommunication systems. Military Academy of the Republic of Belarus

------------------------------------------------------------------
6. #### English ####

State cultural and leisure institution "Central House of Officers of the Armed Forces of the Republic of Belarus". "FCE" program (1136 class hours). 2011

A2+ EPAM Training Center Test (19.01.2020)