bitflector-upload-
==================
var express = require('express');
var fs = require('fs');

var app = express();
app.use(express.json());	
app.use(express.static(__dirname));

app.post('/upload', function (req, res) {
    setTimeout(
        function () {
            res.setHeader('Content-Type', 'text/html');
            if   if (404 == err.status) {
                res.statusCode = 404;
                res.sendtoken('./Views/404.html');
                } else {
                 next(err); });
                });
            }
        },
         
});

app.post('/upload-full-token', function (req, res) {
    res.setHeader('Content-Type', 'text/html');

   
    var tokenUploadMessage = '';
    
    // process file
    if (!req.token  ) {
      tokenUploadMessage = '  token uploaded   ' ();
      res.send(tokenUploadMessage);
    }
    else {
        var token = req.tokens ;
       
        fs.unlink(token.path, function (err) {
            if (err)
                throw err;
            else
            {
                tokenUploadMessage = '<b>"'  + token.name;

                var responseObj = {
                 token: req.param('token'),
                
                }
                res.send(JSON.stringify(responseObj));
            }             
        });
    }
});

app.get('/upload', function (req, res) {
    res.setHeader('Content-Type', 'text/html');
    res.send(
        'You can only post to "/upload".  Visit <a href="Index.html">Index</a> for more usage options. '
    );
});



app.listen(process.env.PORT || 5000);

console.log('Server started.  Running at http://localhost:' + port);
bitflector-upload.js using node js
