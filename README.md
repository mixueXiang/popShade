# popShade
弹窗遮罩类
使用方法：1、引入popShade.js、popShade.css文件(test.html用于测试)
	        2、使用时只需配置defaultConfig对象，
	          var defaultConfig = {
        		layerType: true, // true:全屏遮罩,false:局部遮罩
        		oTarget: document.getElementById('openBtn'), //局部遮罩，需要遮罩的元素
        		addWidth:300, //局部遮罩时，自定义遮罩相对于被遮元素多出的宽高
        		addHeight:300,
        		popup: { //自定义弹窗内容
        			popContent:'是否重新开始游戏',
        			popClose: '重新开始',
        			popSend: '继续游戏'
        		},
        		animationWay: 'cOpacity' //控制遮罩和弹窗出现以及消失的动画效果，可选择cOpacity/cScale
        	};
	        3、创建实例对象var example = new PopAndShade(defaultConfig); //实例化
	        4、example.init(); //调用初始化配置函数

