<h3>一、下载</h3>

<h4>地址：<a href="https://github.com/coreybutler/nvm-windows/releases">https://github.com/coreybutler/nvm-windows/releases</a></h4>

直接选择安装版本即可

<h3>二、安装</h3>

<ol>
<li>运行下载好的 nvm-setup.zip中的安装程序  选择一个盘装到根目录，如 D:\nvm</p></li>
<li><p>检查环境变量是否生成如下变量

<img src="http://upload-images.jianshu.io/upload_images/1750410-509eab5070271e10.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240" alt="1" />
<img src="http://upload-images.jianshu.io/upload_images/1750410-de645d084216f029.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240" alt="2" /></p></li>
<li><p>在cmd中输入：nvm  如出现 Run version .... 即表示安装成功。</p></li>
</ol>

<h3>三、安装node</h3>

<ol>
<li>查看链接，选择要安装的版本 
<a href="https://github.com/coreybutler/nodedistro/blob/master/nodeversions.json">node版本选择</a></li>
<li>cmd输入   nvm install 6.9.3
回车 等待提示是否安装成功</li>
<li>启用node,  cmd输入   nvm use 6.9.3</li>
<li>查看node是否启用成功， cmd输入 node -v</li>
</ol>

<h3>四、总结</h3>

<p>1、 nvm use XXX  切换node版本
2、 nvm list  查看所有已安装node版本

<hr />

<h3>参考链接：<a href="http://www.jianshu.com/p/07c3456e875a" target="_blank">http://www.jianshu.com/p/07c3456e875a</a></h3>