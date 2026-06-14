本项目供北邮学生学习使用，用于下载课程资料(如ppt、pdf、word等)，鉴于油猴的下载插件现在已经不能使用，开发了一种更轻量级的云邮课件下载脚本
# 使用方法
无需安装油猴，将下面代码添加到chrome书签中，打开课件页后，单击书签按钮即可下载

javascript:(function(){let u=decodeURIComponent(location.href),s=u.indexOf('fileucloud.bupt.edu.cn'),e=u.toLowerCase().indexOf('response-content-disposition');if(s>-1)window.location.href='https://'+u.substring(s,e>-1?e:u.length).replace(/[&?F]+$/,'');else alert('请先进入课件预览界面再点击！');})();
