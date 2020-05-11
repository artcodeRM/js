<!DOCTYPE html>
<html>

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>

<body>
    <h1 id="heading">Hello, world!</h1>

    <script src="https://code.jquery.com/jquery-2.1.0.js"></script>
    <script>


        var leftOffset = 0;
        var topOffset = 20;
        var rightOffset = 200;
        var bottomtOffset = 200;

        var moveHeading = function () {
            $("#heading").offset({ left: leftOffset });
            leftOffset++;

            if (leftOffset > 200) {
                clearInterval(1);
                setInterval(moveHeadingTop, 3);
            }
        };
        var moveHeadingTop = function () {
            $("#heading").offset({ top: topOffset });
            topOffset++;

            if (topOffset > 200) {
                clearInterval(2);
                setInterval(moveHeadingRight, 3);
            }
        };
        var moveHeadingRight = function () {
            $("#heading").offset({ left: rightOffset });
            rightOffset--;

            if (rightOffset < 1) {
                clearInterval(3);
                setInterval(moveHeadingBottom, 3);
            }
        };
        var moveHeadingBottom = function () {
            $("#heading").offset({ top: bottomtOffset });
            bottomtOffset--;

            if (bottomtOffset < 1) {

                clearInterval(4);

                leftOffset = 0;
                topOffset = 20;
                rightOffset = 200;
                bottomtOffset = 200;

            }

        };

        var breakHeading = function () {
            leftOffset = 0;
            topOffset = 20;
            rightOffset = 200;
            bottomtOffset = 200;
            setTimeout(moveHeading, 5000);
        }

        setInterval(moveHeading, 3);


    </script>
</body>

</html>
