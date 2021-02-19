<img width=100% style="border-radius: 8px;" src="images/1.gif" />

```csharp
public class Portfolio
{
    private string[] knownLanguages = new[] {
        "C#", "C++", "Java", "PHP", "SQL"
    }

    private string[] myTools = new[] {
        "VSC", "VS2019", "IntelliJ" ,"Firefox"
    }

    private static string[] aboutMe = new[] {
        "Hi, Im Damian also known as L0um15",
        "I am in the 4th grade of IT technical college \n",
        " - 🎂 Im 19 years old",
        " - 🗺️ My native language is Polish.",
        " - 🎵 I Enjoy playing / listening music.",
        " - 😱 I also love to watch horror movies. " +
        "My favourite is Halloween and Nightmare on Elm Street.",
        " - 🔓 I Enjoy contributing to open-source projects.",
        " - 😊 I must say that im a Linux Enthusiast."

    }

    public static void main(String[] args)
    {
        GithubUser me = new GithubUser("https://github.com/L0um15");
        
        for(int i = 0; i < aboutMe.Lenght; i++)
            Console.Writeline(aboutMe[i]);

        for(int i = 0; i < knownLanguages.Lenght; i++){
            Console.Write($"{knownLanguages[i]} ");
        }

        Console.Writeline();

        for(int i = 0; i < myTools.Lenght; i++){
            Console.Write($"{myTools[i]} ");
        }


        while(me.IsInspired()){
            me.GoogleStuff();
            me.ReadDocs();
            me.WriteCode();
            me.HaveFun();
        }
    }

    public static GithubUser GetUser(string url)
        => Github.Connect(url).GetInfo(); 

}
```
<p align=center>
<img alt="L0um15 github stats" src="https://github-readme-stats.vercel.app/api?username=L0um15&theme=radical&show_icons=true&hide_border=true&hide_title=true" />
</p>





