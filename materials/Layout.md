## Layout
### _Layout.cshtml
<img src="https://github.com/keacore/07_RepositoriesViewModels/blob/master/Materials/img/_Layout.png" width="400">    

*_Layout.cshtml*
````Razor  
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>@ViewBag.Title</title>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
    </head>
    <body class="container" style="margin-top: 40px">
        <div class="jumbotron">
            <h1>@ViewBag.Title</h1>
        </div>
            @RenderBody() <!-- All my code from the views will be placed here -->
    </body>
</html>
````   
### Inde.cshtml

````   
@{
    ViewBag.Title = "Students"; // used in the title tag
}
````   

### _ViewStart.cshtml      
    
````CSharp
    @{
         Layout = "~/Views/Shared/_Layout.cshtml";
    }
````   

### Partial View
<img src="https://github.com/keacore/07_RepositoriesViewModels/blob/master/Materials/img/Partial.png" width="400"> 
