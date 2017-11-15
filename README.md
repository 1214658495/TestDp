# TestDp

无论手机屏幕的像素多少，密度比值多少，但80%的手机的dp值(widthPixels / density)都为360dp，所以对于这些手机，我们以360dp为基准，即只要写@dimen/dp_360即可让控件横向沾满屏幕。
故dp值(widthPixels / density)都为360dp，直接拷贝资源文件value里的dimen和其他value—XX就行。

当需要别的dp（540dp），先拷贝资源文件value里的dimen，再拷贝screenMatchDP.jar到main里，再命令行cd到screenMatchDP.jar路径，执行java -jar screenMatchDP.jar 360 384 400 411 533 540 640 720 768 820。就ok了。
