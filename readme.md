function hello(str){

  var split = str.split('')
  var arrays = [];
  var final = [];
  var finished = [];
  var finalSplit = [];
  var yes = ""
  var finalized = ""

 console.log(finished)
  for(var i=0;i<split.length;i++){

    if(i!=0){
      i=i-1
    }
    for(var j=0;j<Math.floor(Math.sqrt(split.length));j++){

        if(i>=Math.floor(Math.sqrt(split.length))){
        arrays[j]+=[split[i]];
        i=i+1
        }else{
           arrays[j]=[split[i]];
        i=i+1
        }
      }
      for(var l=0;l<arrays.length;l++){
          if(l>0){
            finished += arrays[l]
          }else{
            finished = arrays[l]
          }
                   console.log(final)
         final = finished;

      }

  }finalSplit = final.split('')

  for(var m=0;m<finalSplit.length;m++){

    if(m!=0 && m%5===0){
      finalized+=" ";
      finalized+=finalSplit[m]
    }else{
  finalized+=finalSplit[m]
    }
  }return finalized
}

hello("Haveanicedayfeedthedogchilloutand")
