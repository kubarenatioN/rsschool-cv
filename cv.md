# CV in markdown format
1. My fullname is Nikita Kubarko
1. Contacts:
    * Phone: +375 (29) 825-60-42
    * Email: alwayswannaflyinbluesky@gmail.com
1. About me:
   * I love coding. Many people think that programing is a quite hard activity, but i realized that when you study piece by piece it becomes easy to understand almost everything.
   * My goal is to become a front-end developer and get a job on this direction.
   * Every day I try to do something that could make me closer to my purpose, it can be completing labs (C#, markup-languages) for the future, working on course-project or updating my portfolio connected with web-sites development.
   * I can say with confidence that I'am hardworking and self-contained person, sometimes I need a bit of helpful information, but in general I try to solve problems by my own. I always ready to learn something new. Moreover I'm communicative person, it is easy for me to talk with new people, discuss different issues and ways to solve them, I am able to admit my mistakes because I know that mistakes are the only way to grow and upgrade yourself.
1. For now I know and use following technologies and approaches:
   * Perfect knowledge of HTML and CSS
   * Middle-basic JavaScript (event-loop, promises, ajax)
   * Using of npm and gulp to automate the development workflow
   * SASS (CSS-preprocessor)
   * A good knowledge in algorithmization and OOP (C++ and C# labs on github)
   * Using BEM methodology in all projects
   * A good level of English language, can freely speak, write, read
   * Understands of client-server architecture, TCP/IP protocol, ip-addressation, HTTP protocol.
1. Code examples:
   * Reading XML files, using httprequest
    ```javascript
    //Загружаем данные о товарах из файла dataFile.xml в секцию sectionId
    function loadGeneralGoods(dataFile, sectionId) {
      //Возвращаем промис, т.к. используем конструкцию Promise.all().then()
      return new Promise(resolve => {
        //Объект запроса
        let xhttp = new XMLHttpRequest()
        xhttp.onreadystatechange = function () {
          if (this.readyState == 4 && this.status == 200) {
            generalGoodsXmlDataParse(this, sectionId, resolve)
          }
        };
        xhttp.open('GET', 'xml/' + dataFile + '.xml', true)//Формируем характер запроса
        xhttp.send()//Отправляем запрос
      })
    }
    ```
   * overriding the default Enter key behavior in winforms calculator application (lab №1 C#)
    ```csharp
    protected override bool ProcessDialogKey(Keys keyData)
    {
        if (keyData == Keys.Enter)
        {
            string s = label1.Text;//by default s contains equasion
            if (label1.Text.StartsWith("-"))
            {
                s = label1.Text.Remove(0, 1);//if equasion starts with minus -> delete it, and check for operation without it 
            }
            if (!(s.EndsWith("+") || s.EndsWith("-") || s.EndsWith("*") || s.EndsWith("/") || s.EndsWith("%")))
            {
                if (s.Contains('+'))
                {
                    Add();
                }
                ...
                label1.Text = currentResult.ToString();
                isEnterPressed = true;
            }
            return true;
        }
    }
    ```
1. I'm a 2nd-course student of the Belorussian State Technological University (BSTU), on the Faculty of Infomation Technologies (FIT)
1. In my opinion I'm good in English, have a 10 mark for English exam in 3 semester.
