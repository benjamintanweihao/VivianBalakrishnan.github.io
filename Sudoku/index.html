
<html>
<head>

<style>
    p { text-align: center; }
    table { border: 2px solid #000; border-collapse: collapse;
            margin-left: auto; margin-right: auto; }
    input { border: 2px solid #ccc; }
</style>
    
<script type="text/javascript">
    
    function nextfield(me){ 
        var elements=document.getElementsByTagName("input");
			for (i=0; i<elements.length; i++) {
				
				if (elements[i]==me) {
					break;
					}
			}  
		if (isNaN(elements[i].value)) {
					elements[i].value="";
					elements[i].focus();
		}	else	{
        elements[i+1].focus();
        }
    }
    
    
    function draw() {
    	document.write('<table>');
    	for (var row=0; row<9; row++) {
    		document.write('<tr>');
    		for (var col=0; col<9; col++) {
				document.write('<td><input type="text" size="1" maxlength="1" style="font-size:20px" onkeyup="nextfield(this)"/></td>');
			}
			document.write('</tr>');	
    	}
    	document.write('</table>');
    }
  
	
	function SudokuVB() {
								
		BOARD_SIZE = 9;           // Width and height of the SuDoku board
        BOX_SIZE = 3;             // Width and height of the inner boxes
        EMPTY = "";               // Empty cell marker
    	BLANK = 0x0;
		ONES = 0x3fe;
    	var InBlock = [];
		var InRow = [];
		var InCol = [];
		var board = [];
		var Entry = [];
		var Block = [];
		var Row = [];
		var Col = [];
		var Seq = []; 
		var SeqPos = 0; 			  
		
		
		function setup() {
			board = document.getElementsByTagName("input");
     		for (var i=0; i<81; i++) {
     			var Square = i;
     			InRow[Square] = (Math.floor(Square / BOARD_SIZE));
     			InCol[Square] = (Square % BOARD_SIZE);
     			InBlock[Square] = ((Math.floor(Square/27) ) * 3)  + (Math.floor((Square % BOARD_SIZE) / 3));	  		
     		}	   
            
            for (var i=0; i<9; i++) {
            	Block[i] = ONES;
            	Row[i] = ONES;
            	Col[i] = ONES;
		  	}
		
		}
    
    	function bitcount(b){
			b=b>>>1;
			var count = 0;
			while (b) {
				b= (b >>> 1);
				count++;
			}
			return count;
		}
		
		function removeValbit(c,v) {
			Block[InBlock[c]] &= ~v;
			Row[InRow[c]] &= ~v;
			Col[InCol[c]] &= ~v;	
		}
    	
    	function test(SeqNum) {
    		
    		if (SeqNum>=Seq.length) return true;
    	
    		var index = Seq[SeqNum];
    		
			
		  	var possibles = Block[InBlock[index]] & Row[InRow[index]] & Col[InCol[index]];
		  	
		  	while (possibles) {	
		  		
				var valbit = possibles & (-possibles);
				possibles &= ~valbit;
				//Entry[index] = valbit;
				board[index].value = bitcount(valbit);
				
		  		removeValbit(index, valbit);

		  		if (test(SeqNum+1)) return true;
		  		
		  		Block[InBlock[index]] |= valbit;
		  		Row[InRow[index]] |= valbit;
		  		Col[InCol[index]] |= valbit;
		  		}
		  	return false;		 	
		  }		
    
    	this.solve = function() {
             
            setup();
         	for (var i=0; i<81; i++) {	
         		if (board[i].value!=EMPTY) {
         			var valbit2=1<<(board[i].value);
         			removeValbit(i,valbit2);
         		} else {
         			Seq[Seq.length]=i;
         		}
         	}
         	
            if (!test(0))
          		alert("Cannot find solution");     
  		}             
	}	
			        
</script>

</head>


<body>
    
    <table>
      <script type="text/javascript">
      	draw();
        var sd = new SudokuVB();
      </script>
    </table>
    
    <p><button type="button" onclick="sd.solve();">Solve!</button></p>
    
</body>
	
</html>