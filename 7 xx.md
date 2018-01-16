 int[] array = new int[32];
		 int book =0;
		 boolean flag = false;
		 if(x<0){
        	flag = true;
        	x = Math.abs(x);
		 }
		 do{
			 array[book] = (x % 10);
             x /= 10;
             book++;
         }while (x > 0);
         int result = 0;
         int index = 1;
     	StringBuilder resultStr = new StringBuilder ();
         for(int i=0;i<book;i++){
        	 resultStr.append(array[i]);
        	/*if(array[i]==9){
        		System.out.println("array[i]:"+array[i]+";index:"+index+";result:"+result);
        	}*/
        	
         }
         result = Integer.parseInt(resultStr.toString());
         if(flag){
        	 result = -result;
         }
         return result;
