## 在 WSL2 Ubuntu 上安装 OpenGL

Ubuntu 上并不需要安装图形界面。

### 安装依赖库

安装依赖 [^2]

```
sudo apt install mesa-utils libglu1-mesa-dev freeglut3-dev mesa-common-dev
```

### Hello World 程序

在 Ubuntu 上编写以下程序[^1]

```
\*  test.cpp  *\
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

使用命令 `g++ -o test test.cpp -lGL -lGLU -lglut` 编译。

运行命令 `./test` 以测试编译是否成功。

## OpenGL 简介

OpenGL 是应用程序与图形硬件的 API，OpenGL 的核心库提供了 100 多个用于直接访问图形硬件的底层函数。

类似的图形 API 还有 DirectX, GDI.

### OpenGL 开发库组成

- 核心库（GL库）
  - 保护最基本的函数，其前缀是 gl；这部分函数用于常规的、核心的图形处理
  - 由 gl.dll 解释执行

### OpenGL 渲染流水线



## 参考

[^1]: [Linux 下安装 OpenGL](https://blog.csdn.net/csp123258/article/details/82626042)
[^2]: [How to Install OpenGL in Ubuntu in WSL2](https://gist.github.com/Mluckydwyer/8df7782b1a6a040e5d01305222149f3c)