# QSFMLWidget

QSFMLWidget is a widget implementation, based on GNKW's "QSFMLCanvas" abstract class, and implements it as a convinient
ready-to-use widget class along other UI objects, like QOpenGLWidget.

the main aim is to combine the custom SFML draw area with other Qt tools, such as GUI objects etc, rather than replacing 
them with a window fully ocupied with the SFML object.

the meant and easiest way to use the class is:

////////////////////////////////////////////////////////
//mainwindow.cpp
{
    ui->setupUi(this);
    
    QSFMLWidget *drawzone = new QSFMLWidget(this); // default
    drawzone->     /* it's up to you now. be creative :) */
}
////////////////////////////////////////////////////////

alongside your custom changes into qsfmlwidget.h/cpp (functions etc) for your own project,
to call them inide your mainwindow.cpp later.

the use seems pretty similar to QOpenGLWidget introduced in Qt5.4, you can also as well add it to your Qt Designer kit,
use multiple independant drawzones, resize and move them around with regular QWidget functions.

NOTE: The project is very raw, and is kind of a version i uploaded for other people to start off with Qt+SFML 
JUST LIKE I DID MYSELF before writing this.
every experienced user is invited to take a part in it and fix stuff as i will probably do myself after a while
if i even continue with it. Good luck fellas.
