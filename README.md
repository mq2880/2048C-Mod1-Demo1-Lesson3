# 2048C-Mod1-Demo1-Lesson3

# Lesson 3: Creating a Web Application by Using Visual Studio 2017

### Demonstration: Creating a Website by Using Visual Studio 2017

#### Preparation Steps 

1. Ensure that you have cloned the 20480C directory from GitHub **(https://github.com/MicrosoftLearning/20480-Programming-in-HTML5-with-JavaScript-and-CSS3/tree/master/Allfiles)**. It contains the code segments for the labs and demos in this course. 


#### Demonstration Steps

#### Create a website project

1.	Open Microsoft Visual Studio 2017.
2.	In  Microsoft Visual Studio, on the **File** menu, point to **New**, and then click **Project**.
3.	In the **New Project** dialog box, Select **Web**, click **ASP.NET Web Application(.NET Framework)**.

>**Note**: It does not matter whether you select the **Visual Basic** or **Visual C#** templates in the left pane; the templates for both languages enable you to create HTML5 webpages and implement functionality by using JavaScript.

4. In the **Name** text box enter **DemoWebSite**.
5. From the location drop-down list, set the file path to **[Repository Root]\Allfiles\Mod01\Democode\DemoWebSite**, and then click **OK**.
6. In **New ASP.NET Web Application-DemoWebSite**, Select **Empty**, and then click **OK**.

### Add and edit files in the project

1.	In **DemoWebSite - Microsoft Visual Studio**, click **Solution Explorer**.
2.	In Solution Explorer, right-click the **DemoWebSite** project, point to **Add**, and then click **Existing Item**.
3.	In the **Add Existing Item - DemoWebSite** dialog box, browse to **[Repository Root]\Allfiles\Mod01\Democode**, click **ContactUs.html**, and then click **Add**.
4.	In Solution Explorer, right-click **ContactUs.html**, and then click **Set As Start Page**.
5.	In Solution Explorer, right-click the **DemoWebSite** project, point to **Add**, click **New Folder**, and then name it **styles**.
6.	Right-click the **styles** folder, point to **Add**, and then click **New Item**.
7.	In the **Add New Item - DemoWebSite** dialog box, in the middle pane, click **Style Sheet**. In the **Name** box, enter **ContactUsStyles.css**, and then click **Add**.

>**Note**: You can also use the **Add New Item - DemoWebSite** dialog box to create new JavaScript and HTML files and add them to a project.

8. In the **ContactUsStyles.css** file, add the following style:

   ```css
        body {
            font-family: 'Times New Roman';
            color: blue;
        }
   ```

9. In Solution Explorer, double-click **ContactUs.html**.

10. On the page, add the following markup to the **&lt;head&gt;** element:

   ```html
        <head>
            <meta charset="UTF-8" />
            <title>Contact Us</title>
            <link href="styles/ContactUsStyles.css" rel="stylesheet" type="text/css" />
        </head>
   ```

>**Note**: HTML IntelliSense provides hints to help ensure that you enter valid HTML. The **Pick URL** wizard enables you to quickly select a style sheet.

11. On the **File** menu, click **Save All**.

#### Run the web application

1.	In DemoWebSite - Microsoft Visual Studio, on the **Debug** menu, click **Start Debugging**.
2.	If the **Debugging Not Enabled** dialog box appears, click **Modify the Web.config file to enable debugging**, and then click **OK**.
3.	Verify that Microsoft Edge starts running and displays **ContactUs.html**. The text for the page should appear in blue.
4.	In Microsoft Edge, if the **Intranet settings are turned off by default** message appears, click **Don’t show this message again**.

>**Note**: You can enter some sample data, but do not click **Send** because the URL that is the target of the form is not available.


#### Modify the live application

1. Switch to **DemoWebSite - Microsoft Visual Studio**.

2. In the **ContactUs.html** file, make the following modifications:

   - Change **&lt;strong>Name</strong&gt;** to **&lt;strong>Full name</strong&gt;**.
   - Change **Telephone** to **Telephone number**.

3. In the **ContactUsStyles.css** file, add the following style:

   ```css
       h1 {
           font-family: 'Copperplate Gothic';
           color: red;
       }
   ```

4. On the **File** menu, click **Save All**.

5. To refresh the display, return to Microsoft Edge and press F5.

6. Verify that the **Name** field changed to **Full name**, the **Telephone** field changed to **Telephone number**, and that the style of the heading has changed.

7. Return to **DemoWebSite - Microsoft Visual Studio**.

8. On the **Debug** menu, click **Stop Debugging**.