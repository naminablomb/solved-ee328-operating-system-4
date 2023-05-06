Download Link: https://assignmentchef.com/product/solved-ee328-operating-system-4
<br>



<h1>I/O and Simple NetWork Programming</h1>

<h2>1 PROBLEM</h2>

<h3>1.1 DESCRIPTION</h3>

Create a class WGet that takes a URL and a filename on the command line, and attempts to retrievethedataatthatURLintothespecifiedfile. Forexample, “javaWGethttp://www.cs.colum bia.edu/index.html myfile.html”, then you are retrieving the file at CS website and store it into your own file myfile.html.

It should fail if the filename you are trying to write to is already existing, and fail with an informative message if something goes wrong (i.e. don’t just dump a stack trace ).

You can assume that the data is binary, i.e. don’t worry about whether to use a Reader, just use an InputStream. You can also assume the file is text only. Just notify it in your code.

<h2>2 ALGORITHM</h2>

<h3>2.1 INPUT STREAM FROM URL</h3>

InordertoretrievedatafromaURLweusepackage<em>java.net.HttpURLConnection</em>and<em>java.net.URL </em>to found a connection between local machine and web. Then we use the self-implemented method <em>readInputStream() </em>to download data to a local buffer.

<h3>2.2 OUTPUT STREAM TO LOCAL FILE</h3>

In order to save the data to a local file, file I/O stream is useful. We use class <em>FileOutputStream </em>to open an newly-created file, then use method <em>write() </em>to save data to the file. In order to avoid editing an existing file we implement a class <em>ExistingFileException </em>to deal with such circumstances.

1

Figure 3.1: Screenshot of Command Line Window

Figure 3.2: Screenshot of Original Web

<h2>3 RESULTS</h2>

<h3>3.1 ENVIRONMENT</h3>

<ul>

 <li>Windows 10</li>

 <li>Java Development Kit 1.8.0_131</li>

 <li>Eclipse</li>

 <li>Chrome</li>

</ul>

<h3>3.2 SCREENSHOTS OF THE RESULT</h3>

<table>

 <tbody>

  <tr>

   <td width="75"></td>

  </tr>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>

We use command line to compile and execute the program. The result is shown in Fig. 3.1, Fig.

3.2 and Fig 3.3.

<h3>3.3 THOUGHTS</h3>

This project helps us to learn basic skills about web programming in Java. It’s very interesting because it combines web programming and file I/O programming.

Figure 3.3: Screenshot of Local HTML File

2