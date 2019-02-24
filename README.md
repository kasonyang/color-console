![Maven Central](https://img.shields.io/maven-central/v/site.kason/color-console.svg)

# Installation

gradle:

    compile 'site.kason:color-console:$VERSION'


# Usage

    import site.kason.colorconsole.ColorConsole;

    ColorConsole cc = ColorConsole.getDefault();
    cc.info("info message\n");
    cc.warn("err message\n");
    cc.status("testing info ");
    for(int i=0;i<100;i++){
        cc.status("Progress " + i + "%");
        Thread.sleep(200);
    }
    cc.clearStatus();

