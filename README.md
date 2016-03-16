function touming(text){
	if(toumingFlag){
		toumingFlag=false;
		$().toastmessage('showToast', {
			  stayTime : 1000,
	      text     : text,
	      sticky   : false,
	      position : 'middle-center',
				close :function(){
					toumingFlag=true;
				}
	   });
	}
}

使用：touming("输出文本");
