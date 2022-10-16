```cs
using System.Text;

namespace Github 
{
    internal class Profile
    {
        string name;
        int age;
        string[] hobbies;
        
        public Profile(string name, int age, string[] hobbies)
        {
            this.name = name;
            this.age = age;
            this.hobbies = hobbies;
        }
        
        string DisplayName()
        {
            return $"My name is {name}";
        }
        
        string DisplayAge()
        {
            return $"I have been on this planet for around {age*365} days";
        }
        
        string DisplayHobbies()
        {
            StringBuilder hobbyText = new StringBuilder("Some of my hobbies include:");
            foreach(string hobby in hobbies)
            {
                hobbyText.Append($"\n ○ {hobby}");
            }
            return hobbyText.ToString();
        }
        
        public override string ToString()
        {
            return $"{DisplayName()}\n{DisplayAge()}\n\n{DisplayHobbies()}";
        }
    }
}

```

My name is Jeet
</break>
I have been on this planet for around 6205 days

Some of my hobbies include:

 `○ Making apps using .NET framework with WPF`
 </break>
 `○ Developing games in unity with C#`
 </break>
 `○ Programming in Python/C#`
 </break>
 `○ Using the p5.js module in javascript to create simple procedural effects`
 </break>
 `○ Learning about Neural Networking`



