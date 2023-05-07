Download Link: https://assignmentchef.com/product/solved-lab-2-asynchronous-simple-http-stock-monitor-stock-monitor-v2
<br>
<strong>IMPORTANT. </strong>You must save all your work in a way that you are able to present them to teacher during the evaluation discussion. You could use for instance GIT. You also need to have working developer environment where you can run the assignments.

<h1>1.    Asynchronous Simple HTTP</h1>

On previous week’s assignments we had to do a little ”hack” to get rid of the Android’s security policy. Today we are going to fix that and do things right.

We have to change our code to work asynchronously. In practice this means that we are several thing in parallel. For example, UI is fully functional at the same time when we are loading something from the network. This was not the case on previous week’s assignment. If we would have loaded large files, the UI would be totally jammed during the loading.

There are several ways to solve this problem and today we are going to use AsyncTask to solve it.

Read first AsyncTask documentation: <a href="https://developer.android.com/reference/android/os/AsyncTask">https://developer.android.com/reference/android/os/AsyncTask</a>

Create a new app with same style as previous Simple HTTP and use AsyncTask to load data asynchronously. Remove the<strong> StrictMode.ThreadPolicy </strong>code to make sure that your load is asynchronous.

<h1>2.    Stock Monitor</h1>

Create an app which can be used as stock monitor.

First version of the app should display stock prices of following companies

<table width="395">

 <tbody>

  <tr>

   <td width="198"><strong>Company</strong></td>

   <td width="198"><strong>Stock ID</strong></td>

  </tr>

  <tr>

   <td width="198">Apple</td>

   <td width="198">AAPL</td>

  </tr>

  <tr>

   <td width="198">Alphabet (Google)</td>

   <td width="198">GOOGL</td>

  </tr>

  <tr>

   <td width="198">Facebook</td>

   <td width="198">FB</td>

  </tr>

  <tr>

   <td width="198">Nokia</td>

   <td width="198">NOK</td>

  </tr>

 </tbody>

</table>




Use this REST api to get the stock price: <a href="https://financialmodelingprep.com/api/company/price/NOK">https://financialmodelingprep.com/api/company/price/NOK</a> Last parameter in the path will be the stock ID.

Api returns the result in JSON format. You can test it in browser to see the format. We haven’t yet studied elegant ways to parse JSON, we will do it next week. Today you can do JSON parsing (get the price out of the json) with Java’s <strong>String</strong> methods <strong>indexOf</strong> and <strong>subString. </strong>Of course, you can use more elegant json parsers if you wish.

Here’s the example of the UI.

<h1>3.    Stock Monitor V2</h1>

Create a copy of the previous stock monitor app. Modify it in a way that you can add more stocks to the app. See the example below.

<em> </em>