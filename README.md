# three.js learning
## 简介
Three.js是一个基于JavaScript编写的开源3D图形库，利用WebGL技术在网页上渲染3D图形。它提供了许多高级功能，如几何体、纹理、光照、阴影等，以便开发者能够快速地创建复杂且逼真的3D场景。同时，Three.js还具有很好的跨平台和跨浏览器兼容性，让用户无需安装任何插件就可以在现代浏览器上观看3D内容。
[链接](https://threejs.org/)
## Three.js 程序结构
### 场景Scene
创建场景
`const scene = new THREE.Scene();`
#### 网格模型Mesh
**几何体**
创建几何体
··
形状
尺寸
**材质**
颜色
贴图
透明度
#### 光照Light
**颜色**
**分类**
环境光
点光源
平行光
### 相机Camera
创建透视相机(fov视场角度、aspect宽高比、near近平面的距离、far远平面的距离)
`const camera = new THREE.PerspectiveCamera(fov,aspect,near,far);`
**位置Position**
**视线方向.lookAT()**
**投影方式**
透射投影PerspectiveCamera
正射投影OrthographicCamera
### 渲染器Renderer
创建WebGL渲染器
```
const renderer = new THREE.WebGLRenderer();
renderer.setSize(window.innerWidth,window.innerHeight);
document.body.appendChild(renderer.domElement);
```
**渲染器创建**
WebGLRenderer()
**开始渲染**
.render(scene,camera)
**domElement属性**
Canvas对象


