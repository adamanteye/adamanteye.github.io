## 在 WSL2 Ubuntu 上安装 OpenGL

Ubuntu 上并不需要安装图形界面。

### 安装依赖库

安装依赖 [^2]

```
sudo apt install mesa-utils libglu1-mesa-dev freeglut3-dev mesa-common-dev
```

### Hello World 程序

在 Ubuntu 上编写以下程序

```
\*  test.c  *\
#include <GL/glut.h>

void init(void)
{
    glClearColor(0.0, 0.0, 0.0, 0.0);
    glMatrixMode(GL_PROJECTION);
    glOrtho(-5, 5, -5, 5, 5, 15);
    glMatrixMode(GL_MODELVIEW);
    gluLookAt(0, 0, 10, 0, 0, 0, 0, 1, 0);

    return;
}

void display(void)
{
    glClear(GL_COLOR_BUFFER_BIT);
    glColor3f(1.0, 0, 0);
    glutWireTeapot(3);
    glFlush();

    return;
}

int main(int argc, char *argv[])
{
    glutInit(&argc, argv);
    glutInitDisplayMode(GLUT_RGB | GLUT_SINGLE);
    glutInitWindowPosition(0, 0);
    glutInitWindowSize(300, 300);
    glutCreateWindow("OpenGL 3D View");
    init();
    glutDisplayFunc(display);
    glutMainLoop();

    return 0;
}
```

使用命令 `gcc -o test test.c -lGL -lGLU -lglut` 编译 [^1]

## 参考

[^1]: [Linux 下安装 OpenGL](https://blog.csdn.net/csp123258/article/details/82626042)
[^2]: [How to Install OpenGL in Ubuntu in WSL2](https://gist.github.com/Mluckydwyer/8df7782b1a6a040e5d01305222149f3c)