# Module02-reflection
***
Ngày 22-02-2021<br>
Bài 14 - Reflection
<dl>
<dt>-Chuỗi (String)</dt>
<dd>+Chuỗi là một kiểu dữ liệu cơ bản trong PHP. Chuỗi là dãy liên tiếp các ký tự. Chuỗi mà không chứa ký tự thì được gọi là chuỗi rỗng.</dd>
<dd>+Chuỗi được bao quanh bởi dấu nháy đơn (' ') hoặc dấu nháy kép (" "). Sau đây là một vài ví dụ về chuỗi hợp lệ trong PHP</dd>
<dt>-Các hàm thao tác với chuỗi</dt>
<dd>+strlen($string): hàm trả về độ dài chuỗi</dd>
<dd>+str_word_count($string): hàm trả về số từ trong chuỗi</dd>
<dd>+strrev($string): hàm đảo ngược chuỗi</dd>
<dd>+strpos($string,$text): hàm tìm kiếm chuỗi $text trong chuỗi $string. Nếu tìm thấy, hàm trả về chỉ số ký tự đầu tiên tìm thấy của chuỗi. Nếu không tìm thấy, hàm trả về FALSE.</dd>
<dd>+str_replace($find, $replace, $string): hàm tìm kiếm chuỗi $find, thay thế chuỗi đó bằng $replace trong chuỗi ban đầu $string</dd>
<dd>+substr(string,start,length): Hàm này có tác dụng cắt chuỗi $string, bắt đầu ở vị trí $strat và có giới hạn $length</dd>
<dt>-Regular Expression / Regex - Biểu thức chính quy</dt>
<dd>+Biểu thức chính quy (Regular Expression)  thường được gọi là Regex hoặc RegExp. Là thuật toán khớp mẫu mạnh mẽ có thể được thực hiện trong một biểu thức. Nó giúp bạn trong tiết kiệm được rất nhiều thời gian khi xây dựng các trang web động.</dd>
<dt>-Biểu thức chính quy là</dt>
<dd>+Biểu thức chính quy là một nhóm các ký tự, ký hiệu nó được sử dụng để tìm kiếm văn bản (text).</dd>
<dd>+Một biểu thức chính quy là một mẫu nó tương đồng quy luật với một chuỗi từ trái qua phải. Biểu thức chính quy tên tiếng anh là Regular Expression  thường gọi tắt là regex hoặc regexp</dd>
<dd>+Trong lập trình nó được dùng với các hàm xử lý chuỗi, xử lý văn bản với các tác vụ cụ thể như: tìm và thay thế chuỗi, kiểm tra tính hợp lệ của dữ liệu, trích xuất chuỗi con từ một chuỗi ... </dd>
<dt>-Tại sao lại sử dụng biểu thức chính quy</dt>
<dd>+Biểu thức chính quy đơn giản hóa việc xác định các mẫu trong chuỗi dữ liệu bằng cách gọi một hàm duy nhất. Điều này giúp chúng ta tiết kiệm thời gian lập trình.</dd>
<dd>+Khi xác thực đầu input của người dùng nhập vào như username, password, email, tên miền, số điện thoại, địa chỉ IP...</dd>
<dd>+Highlight từ khóa trong kết quả tìm kiếm.</dd>
<dd>+Khi tạo mẫu HTML tùy chỉnh. Biểu thức chính quy thông thường có thể được sử dụng để xác định các tag và thay thế chúng bằng dữ liệu thực tế.</dd>
<dd>+Đặc biệt, sử dụng biểu thức chính quy tăng performance của chương trình rất nhiều lần.</dd>
<dt>- Các hàm thao tác với Regular Expression trong PHP</dt>
<dd>+Hàm preg_match() được dùng để kiểm tra, so khớp và lấy kết quả của việc so sánh chuỗi dựa vào biểu thức chính quy. Hàm trả về TRUE/FALSE. </dd>
<dd>+preg_match_all() cũng tương tự hàm preg_match() ở trên , tuy nhiên hai hàm này khác nhau ở chỗ , hàm preg_match_all() sẽ trả về toàn bộ các giá trị được so sánh khớp, còn hàm preg_match() chỉ trả về giá trị đầu tiên được so sánh khớp.</dd>
<dd>+Sử dụng hàm pre_split để chia nhỏ chuỗi thành mảng chứa các chuỗi con.</dd>
<dd>+Hàm preg_replace dùng để tìm kiếm và thay thế một chuỗi nào đó khớp với đoạn Regular Expression truyền vào. </dd>
</dl>
***<br>
Ngày 19-02-2021<br>
Bài 13 - Reflection
<dl>
<dt>-Xử lý ngoại lệ</dt>
<dd>+Xử lý ngoại lệ được sử dụng để thay đổi luồng chương trình khi xảy ra một lỗi bất thường mà người lập trình không kiểm soát được.</dd>
<dd>VD:</dd>
<dd>+Trạng thái code hiện tại được lưu.</dd>
<dd>+Việc thực thi code sẽ chuyển sang một hàm xử lý ngoại lệ được xác định trước (tùy chỉnh).</dd>
<dd>+Tùy thuộc vào tình huống, trình xử lý có thể tiếp tục thực hiện từ trạng thái mã đã lưu, chấm dứt thực thi tập lệnh hoặc tiếp tục tập lệnh từ một vị trí khác trong tập lệnh.</dd>
<dt>-Các phương thức xử lý ngoại lệ trong PHP:</dt>
<dd>+Sử dụng try, throw và catch.</dd>
<dd>+Tạo lớp ngoại lệ tùy chỉnh.</dd>
<dd>+Xử lý nhiều ngoại lệ.</dd>
<dd>+Ném lại một ngoại lệ.</dd>
<dd>+Thiết lập trình xử lý ngoại lệ cao cấp.</dd>
<dt>-Sử dụng try, throw và catch</dt>
<dd>+try - Một hàm sử dụng ngoại lệ phải ở trong khối "try". Nếu ngoại lệ không xảy ra, code sẽ tiếp tục như bình thường. Tuy nhiên, nếu ngoại lệ xảy ra, ngoại lệ bị "throw".</dd>
<dd>+throw - Đây là cách bạn kích hoạt ngoại lệ. Mỗi "throw" phải có ít nhất một "try".</dd>
<dd>+catch - Một khối "catch" bắt một ngoại lệ và tạo một đối tượng chứa thông tin ngoại lệ.</dd>
<dd>VD:</dd>
<dd><pre><?php
//tạo hàm và throw một ngoại lệ
function checkNum($number) {
  if($number > 1) {
    throw new Exception("Giá trị phải nhỏ hơn hoặc bằng 1.");
  }
  return true;
}
 
//kích hoạt ngoại lệ trong khối "try"
try {
  checkNum(2);
  // nếu ngoại lệ được ném ra thì lệnh sau không được thực thi
  echo 'Number nhỏ hơn hoặc bằng 1.';
}
 
//catch exception
catch(Exception $e) {
  echo 'Message: ' .$e->getMessage();
}
?></pre></dd>
<dt>-Tạo một lớp ngoại lệ tùy chỉnh</dt>
<dd>+Để tạo một trình xử lý ngoại lệ tùy chỉnh, bạn phải tạo một lớp đặc biệt với các hàm có thể được gọi khi một ngoại lệ xảy ra trong PHP. Lớp này phải được kế thừa lớp Exception.</dd>
<dd>+Lớp ngoại lệ tùy chỉnh kế thừa các thuộc tính từ lớp Exception của PHP và bạn có thể thêm các hàm tùy chỉnh vào nó.</dd>
<dd>VD:</dd>
<dd><pre><?php
class CustomException extends Exception {
  public function errorMessage() {
    //error message
    $errorMsg = 'Error on line '.$this->getLine().' in '.$this->getFile()
        .': <b>'.$this->getMessage().'</b> is not a valid E-Mail address';
    return $errorMsg;
  }
}
 
$email = "someone@example...com";
 
try {
  //check email hợp lệ
  if(filter_var($email, FILTER_VALIDATE_EMAIL) === FALSE) {
    //throw exception nếu email không hợp lệ
    throw new customException($email);
  }
}
 
catch (customException $e) {
  //hiển thị message
  echo $e->errorMessage();
}
?></pre></dd>
<dd>+Lớp mới là một bản sao của lớp Exception cũ với việc bổ sung hàm errorMessage(). Vì nó là một bản sao của lớp cũ, và nó kế thừa các thuộc tính và phương thức từ lớp cũ, chúng ta có thể sử dụng các phương thức lớp Exception như getLine() và getFile() và getMessage().</dd>
<dt>-Quy tắc cho trường hợp ngoại lệ</dt>
<dd>+Code nên được đặt trong khối try, để giúp bắt (catch) các ngoại lệ có thể xảy ra.</dd>
<dd>+Mỗi khối try hoặc "throw" phải có ít nhất một khối catch tương ứng.</dd>
<dd>+Nhiều khối catch có thể được sử dụng để bắt các lớp ngoại lệ khác nhau.</dd>
<dd>+Có thể ném các ngoại lệ (hoặc được ném lại) vào khối catch trong khối try.</dd>
</dl>
***<br>
Ngày 18-02-2021<br>
Bài 12 - Reflection
<dl>
 <dt>-Thuật toán sắp xếp</dt>
  <dd>+Sắp xếp (sorting) là quá trình bố trí lại các phần tử của một danh sách các đối tương nào đó theo một trật tự nhất định. Chẳng hạn tứ tự tăng dần (hay giảm dần) đối với một dãy số, thứ tự từ điển đối với một dãy chữ...</dd>
  <dt>-Giải thuật sắp xếp In-place và Not-in-place</dt>
  <dd>+Những giải thuật mà không yêu cầu thêm bất kỳ bộ nhớ phụ và việc sắp xếp được tiến hành trong chính phần bộ nhớ đã khai báo trước đó (ví dụ trong một mảng chẳng hạn) thì được gọi là in-place sorting. Ví dụ cho loại giải thuật sắp xếp này là giải thuật sắp xếp nổi bọt (bubble sorting).</dd>
  <dd>+Nhưng trong một số giải thuật sắp xếp, chương trình cần thêm lượng bộ nhớ mà có thể lớn hơn hoặc bằng với số phần tử đang được sắp xếp. Các giải thuật này được gọi là not-in-place sorting. Ví dụ cho loại giải thuật này là sắp xếp trộn (merge sort).</dd>
  <dt>-Giải thuật sắp xếp Adaptive và Non-Adaptive</dt>
  <dd>+Một giải thuật được xem như là adaptive, nếu nó tận dụng các phần tử đã được sắp xếp trong danh sách mà đã được sắp xếp. Đó là, trong khi sắp xếp nếu danh sách ban đầu có một số phần tử đã được sắp xếp, thì giải thuật dạng adaptive sẽ ghi nhận các phần tử này và sẽ cố gắng không thay đổi thứ tự của chúng.</dd>
  <dd>+Trái ngược với loại giải thuật trên, giải thuật dạng non-adaptive sẽ không ghi nhận các phần tử đã được sắp xếp trước đó. Giải thuật loại này sẽ vấn cố gắng sắp xếp lại từng phần tử trong danh sách ban đầu.</dd>
  <dt>-Các khái niệm quan trọng trong giải thuật sắp xếp</dt>
  <dd>+Thứ tự tăng</dd>
  <dd>+Thứ tự giảm</dd>
  <dd>+Thứ tự không tăng</dd>
  <dd>+Thứ tự không giảm</dd>
  <dt>-Sắp xếp nổi bọt (Bubble Sort)</dt>
  <dd>+Sắp xếp nổi bọt là một giải thuật sắp xếp đơn giản. Giải thuật sắp xếp này được tiến hành dựa trên việc so sánh cặp phần tử liền kề nhau và tráo đổi thứ tự nếu chúng không theo thứ tự.</dd>
  <dd>+Giải thuật này không thích hợp sử dụng với các tập dữ liệu lớn khi mà độ phức tạp trường hợp xấu nhất và trường hợp trung bình là Ο(n2) với n là số phần tử.</dd>
  <dd>Vd:</dd>
  <dd><pre>Bắt đầu hàm bubbleSort( list : mảng các phần tử )

   loop = list.count;
   
   for i = 0 tới loop-1 thực hiện:
      swapped = false
		
      for j = 0 tới loop-1 thực hiện:
      
         /* so sánh các phần tử cạnh nhau */   
         if list[j] > list[j+1] then
            /* tráo đổi chúng */
            swap( list[j], list[j+1] )		 
            swapped = true
         kết thúc if
         
      kết thúc for
      
      /*Nếu không cần tráo đổi phần tử nào nữa thì 
      tức là mảng đã được sắp xếp. Thoát khỏi vòng lặp.*/
      
      if(not swapped) then
         break
      kết thúc if
      
   kết thúc for
   
Kết thúc hàm return list</pre></dd>
<dt>-Sắp xếp chèn (Insertion Sort)</dt>
<dd>+Sắp xếp chèn là một giải thuật sắp xếp dựa trên so sánh in-place. Ở đây, một danh sách con luôn luôn được duy trì dưới dạng đã qua sắp xếp. Sắp xếp chèn là chèn thêm một phần tử vào danh sách con đã qua sắp xếp. Phần tử được chèn vào vị trí thích hợp sao cho vẫn đảm bảo rằng danh sách con đó vẫn sắp theo thứ tự.</dd>
<dd>+Với cấu trúc dữ liệu mảng, chúng ta tưởng tượng là: mảng gồm hai phần: một danh sách con đã được sắp xếp và phần khác là các phần tử không có thứ tự. Giải thuật sắp xếp chèn sẽ thực hiện việc tìm kiếm liên tiếp qua mảng đó, và các phần tử không có thứ tự sẽ được di chuyển và được chèn vào vị trí thích hợp trong danh sách con (của cùng mảng đó).</dd>
<dd>+Giải thuật này không thích hợp sử dụng với các tập dữ liệu lớn khi độ phức tạp trường hợp xấu nhất và trường hợp trung bình là Ο(n2) với n là số phần tử.</dd>
<dd>VD:</dd>
<dd><pre>function insertion_Sort($my_array)
{
    for($i=0;$i<count($my_array);$i++){
        $val = $my_array[$i];
        $j = $i-1;
        while($j>=0 && $my_array[$j] > $val){
            $my_array[$j+1] = $my_array[$j];
            $j--;
        }
        $my_array[$j+1] = $val;
    }
    return $my_array;
}</pre></dd>
  <dt>-Giải thuật sắp xếp chọn (Selection Sort)</dt>
  <dd>+Giải thuật sắp xếp này là một giải thuật dựa trên việc so sánh in-place, trong đó danh sách được chia thành hai phần, phần được sắp xếp (sorted list) ở bên trái và phần chưa được sắp xếp (unsorted list) ở bên phải. Ban đầu, phần được sắp xếp là trống và phần chưa được sắp xếp là toàn bộ danh sách ban đầu.</dd>
  <dd>+Phần tử nhỏ nhất được lựa chọn từ mảng chưa được sắp xếp và được tráo đổi với phần bên trái nhất và phần tử đó trở thành phần tử của mảng được sắp xếp. Tiến trình này tiếp tục cho tới khi toàn bộ từng phần tử trong mảng chưa được sắp xếp đều được di chuyển sang mảng đã được sắp xếp.</dd>
  <dd>+Giải thuật này không phù hợp với tập dữ liệu lớn khi mà độ phức tạp trường hợp xấu nhất và trường hợp trung bình là O(n2) với n là số phần tử.</dd>
  <dd>VD:</dd>
  <dd><pre>Bắt đầu giải thuật sắp xếp chọn (Selection Sort) 
   list  : mảng các phần tử
   n     : kích cỡ mảng

   for i = 1 tới n - 1
   /* thiết lập phần tử hiện tại là min*/
      min = i    
  
      /* kiểm tra phần tử có là nhỏ nhất không */

      for j = i+1 tới n 
         if list[j] < list[min] thì
            min = j;
         kết thúc if
      kết thúc for

      /* tráo đổi phần tử nhỏ nhất với phần tử hiện tại*/
      if indexMin != i  then
         tráo đổi list[min] và list[i]
      kết thúc if

   kết thúc for
	
Kết thúc giải thuật</pre></dd>
</dl>
***<br>
Ngày 18-02-2021 <br>
Bài 11 - Reflection
<dl>
<dt>-Thuật toán tìm kiếm tuyến tính</dt>
  <dd>+Linear Search là một giải thuật tìm kiếm rất cơ bản. Trong kiểu tìm kiếm này, một hoạt động tìm kiếm liên tiếp được diễn ra qua tất cả từng phần tử. Mỗi phần tử đều được kiểm tra và nếu tìm thấy bất kỳ kết nối nào thì phần tử cụ thể đó được trả về; nếu không tìm thấy thì quá trình tìm kiếm tiếp tục diễn ra cho tới khi tìm kiếm hết dữ liệu.</dd>
  <dt>Vd:</dt>
  <dd><pre>$numbers = range(1, 200, 5);

if (search($numbers, 31)) { 
    echo "Found"; 
} else { 
    echo "Not found"; 
}</pre>
</dd>
<dt>-Thuật toán tìm kiếm nhị phân</dt>
<dd>+Binary Search tìm kiếm một phần tử cụ thể bằng cách so sánh phần tử tại vị trí giữa nhất của tập dữ liệu. Nếu giá trị trùng nhau thì chỉ mục của phần tử được trả về. Nếu phần tử cần tìm là lớn hơn giá trị phần tử giữa thì phần tử cần tìm được tìm trong mảng con nằm ở bên phải phần tử giữa; nếu không thì sẽ tìm ở trong mảng con nằm ở bên trái phần tử giữa. Tiến trình sẽ tiếp tục như vậy trên mảng con cho tới khi tìm hết mọi phần tử trên mảng con này.</dd>
<dt>Vd:</dt>
<dd><pre>$numbers = range(1, 200, 5); 

$number = 31;
if (binarySearch($numbers, $number) !== FALSE) { 
    echo "$number Found \n"; 
} else { 
    echo "$number Not found \n"; 
} 

$number = 500; 
if (binarySearch($numbers, $number) !== FALSE) { 
    echo "$number Found \n"; 
} else { 
    echo "$number Not found \n"; 
}</pre> </dd>
</dl>
***<br>
Ngày 05/02/2021<br>
Bài 10 - Reflection
<dl>
<dt>SPL là bộ thư viên chuẩn của PHP, nó gồm tập hợp các interface, abstract class nhằm giải quyết các bài toán phổ biên.</dt>
  <dd>-Các thành phần của SPL</dd>
  <dd>+Predefined Constants là danh sách các hằng số :số pi, số E,...</dd>
  <dd>+Datastructures chứa danh sách các lớp co khả năng làm việc với cấu trúc, dữ liệu khác nhau LinkList, Stack, Queue, Heaps,...</dd>
  <dd>+Interator: Chứa các lớp cho phép có khả năng thực hiện các phép lặp để duyệt các cấu trúc khác nhau tùy vào cấu trúc dữ liệu.</dd>
  <dd>+Danh sách các Interface</dd>
  <dd>+Exception là danh sách điều khiển các lớp ngoại lệ</dd>
  <dd>+File Handling cung cấp các lớp làm việc với file trong hệ thống.</dd>
  <dd>+SPL Funtions cung cấp các hàm hỗ trợ cần thiết.</dd>
  <dd>+Miscellaneous Classes và Interface.</dd>
</dl>
<dl>Các loại cấu trúc dữ liệu: -PHP DATASTRUCTURES
<dt>-DoublyLinkedList:</dt>
  <dd>+Là một danh sách liên kết đôi, các node được liên kết với nhau theo hai hướng.</dd>
  <dd>+PHP cung cấp sẵn các lớp SplDoublyLinkedList là SplStack và SplQueue</dd>
  <dt>-HEAP là một dạng cấu trúc gần như Tree, trong đó mỗi node có giá trị lớn hơn hoặc bằng các node con của nó.</dt>
  <dd>+PHP cung cấp sẵn các lớp thuộc Heaps bao gồm SplHeap và SplPriorityQueue.Trong SplHeap có SplMaxHeap và SplMinHeap</dd>
  <dt>-ARRAYS là cấu trúc dữ liệu trong đó lưu trữ các phần tử theo hình thức liên tiếp nhau , truy cập dựa theo chỉ số.</dt>
  <dd>+PHP cung cấp lớp có sẵn SplFixedArray</dd>
  <dd>+Lưu ý cấu trúc Arrays khác khái niệm mảng trong PHP.Mảng trong PHP được triển khai theo hình thức Hashtable có trật tự.</dd>
  <dt>-MAP là cấu trúc dữ liệu trong đó các phần tử được quản lý theo cặp key-value.</dt>
  <dd>+PHP cung cấp lớp SplObjectStorage</dd>
  <dd>+Mảng trong PHP cũng có thể coi là cấu trúc Map.Trong đó key có kiểu dữ liệu là int hoặc string.</dd>
</dl>
***<br>
Ngày 04/02/2021<br>
Bài 9 - Reflection
<dl>
<dt>-Cấu trúc dữ liệu ngăn xếp (Stack)</dt>
  <dd>+Đặc điểm là làm cho ngăn xếp trở thành cấu trúc dữ liệu dạng LIFO. LIFO là viết tắt của Last-In-First-Out. Ở đây, phần tử được đặt vào (được chèn, được thêm vào) cuối cùng sẽ được truy cập đầu tiên. </dd>
  <dt>-Các hoạt động cơ bản trên cấu trúc dữ liệu ngăn xếp</dt>
  <dd>+Hoạt động push(): lưu giữ một phần tử trên ngăn xếp.</dd>
  <dd>+Hoạt động pop(): xóa một phần tử từ ngăn xếp.</dd>
  <dd>+Hoạt động peek(): lấy phần tử dữ liệu ở trên cùng của ngăn xếp, mà không xóa phần tử này.</dd>
  <dd>+Hoạt động isFull(): kiểm tra xem ngăn xếp đã đầy hay chưa.</dd>
  <dd>+Hoạt động isEmpty(): kiểm tra xem ngăn xếp là trống hay không.</dd>
</dl>
<dl>
<dt>-Cấu trúc dữ liệu hàng đợi (Queue)</dt>
  <dd>+Một đầu luôn luôn được sử dụng để chèn dữ liệu vào (hay còn gọi là sắp vào hàng) và đầu kia được sử dụng để xóa dữ liệu (rời hàng). Cấu trúc dữ liệu hàng đợi tuân theo phương pháp First-In-First-Out, tức là dữ liệu được nhập vào đầu tiên sẽ được truy cập đầu tiên.</dd>
  <dt>-Các hoạt động cơ bản trên cấu trúc dữ liệu hàng đợi</dt>
  <dd>+Hoạt động enqueue(): thêm (hay lưu trữ) một phần tử vào trong hàng đợi.</dd>
  <dd>+Hoạt động dequeue(): xóa một phần tử từ hàng đợi.</dd>
  <dd>+Phương thức peek(): lấy phần tử ở đầu hàng đợi, mà không xóa phần tử này.</dd>
  <dd>+Phương thức isFull(): kiểm tra xem hàng đợi là đầy hay không.</dd>
  <dd>+Phương thức isEmpty(): kiểm tra xem hàng đợi là trống hay hay không.</dd>
</dl>
<dl>
<dt>-Cấu trúc cây (tree)</dt>
  <dd>+Cấu trúc Tree hoạt động theo nguyên tắc phân cấp, trong đó có mối quan hệ cha-con giữa các nút (node). Node mà không có cha thì được gọi là root (nút gốc), node mà không có con thì được gọi là leaf (nút lá). Những node có chung cha thì được gọi là siblings (anh em). Khái niệm edges (cạnh) được dùng để chỉ đến đường kết nối giữa các node.</dd>
  <dt>-Thêm node vào trong Tree</dt>
  <dd>+Đây là một cách triển khai đơn giản, theo chiến thuật "chia để trị"</dd>
  <dd>+Tất cả những phần tử nhỏ hơn phần tử hiện tại thì chuyển sang bên trái, tất cả những phần tử lớn hơn thì chuyển sang bên phải, tất cả những phần tử trùng lặp (đã tồn tại trước đó) thì sẽ bị từ chối (không thêm vào)</dd>
  <dt>Duyệt qua các phần tử của tree</dt>
  <dd>+pre-order - duyệt node hiện tại rồi sau đó sang cây bên trái và cây bên phải</dd>
  <dd>+in-order (đối xứng) - duyệt bên trái trước, sau đó duyệt node hiện tại, rồi duyệt node bên phải</dd>
  <dd>+post-order - duyệt bên trái trước, sau đó bên phải, rồi duyệt node hiện tại</dd>
  <dd>+level-order (duyệt theo bề rộng) - duyệt node hiện tại, sau đó duyệt tất cả các node anh em (siblings), rồi chuyển sang duyệt những node ở level tiếp theo</dd>
</dl>
***<br>
Ngày 03/02/2021<br>
Bài 8 - Reflection
<dl>
<dt>-Cấu trúc dữ liệu là hình thức tổ chức một nhóm dữ liệu bao gồm các chức năng:</dt>
  <dd>+Lưu trữ dữ liệu</dd>
  <dd>+Cung cấp các phương thức để thao tác với dữ liệu.</dd>
  <dt>-Các cấu trúc dữ liệu thông dụng</dt>
  <dd>Set (Tập hợp): Nhóm các phần tử không trùng nhau</dd>
  <dd>List (Danh sách): Nhóm ác phần tử có thể trùng nhau</dd>
  <dd>Stack: Nhóm các phần tử theo trật tự first-in/last-out (vào trước/ra sau)</dd>
  <dd>Queue: Nhóm các phần tử theo trật tự first-in/first-out (vào trước/ra trước)</dd>
  <dd>Map (Bản đồ): Lưu trữ các cặp key/value</dd>
  <dd>Tree (Cây): Lưu trữ các phần tử theo mối quan hệ cha-con</dd>
  <dd>Graph (Đồ thị): Lưu trữ các phần tử theo mối quan hệ mạng lưới</dd>
</dl>
<dl> ArrayList
<dt>-Mảng có thể lưu giữ một số phần tử cố định và các phần tử này nền có cùng kiểu.</dt>
  <dt>-Ưu điểm</dt>
  <dd>+Truy câp phàn tử vơi thời gian hằng số O(1)</dd>
  <dd>+Sử dụng bộ nhớ hiệu quả</dd>
  <dd>+Tính cục bộ về bộ nhớ</dd>
  <dt>-Nhược điểm</dt>
  <dd>+Không thể thay đổi kích thước của mảng khi chương trình dang thực hiện</dd>
  <dt>-Phép toán cơ bản được hỗ trợ bởi mảng</dt>
  <dd>+Duyệt: In tất cả các phần tử mảng theo cách in từng phần tử một.</dd>
  <dd>+Chèn: Thêm một phần tử vào mảng tại chỉ mục đã cho.</dd>
  <dd>+Xóa: Xóa một phần tử từ mảng tại chỉ mục đã cho.</dd>
  <dd>+Tìm kiếm: Tìm kiếm một phần tử bởi sử dụng chỉ mục hay bởi giá trị.</dd>
  <dd>+Cập nhật: Cập nhật giá trị một phần tử tại chỉ mục nào đó.</dd>
</dl>
<dl>Linked List
<dt>-Danh sách liên kết là một cấu trúc dữ liệu bao gồm một nhóm các nút (node) tạo thành một chuỗi. Mỗi nút gồm dữ liệu ở nút đó và tham chiếu đến nút kế tiếp trong chuỗi.</dt>
  <dt>-Các loại Danh sách liên kết (Linked List)</dt>
  <dd>+Danh sách liên kết đơn (Simple Linked List): chỉ duyệt các phần tử theo chiều về trước.</dd>
  <dd>+Danh sách liên kết đôi (Doubly Linked List): các phần tử có thể được duyệt theo chiều về trước hoặc về sau.</dd>
  <dd>+Danh sách liên kết vòng (Circular Linked List): phần tử cuối cùng chứa link của phần tử đầu tiên như là next và phần tử đầu tiên có link tới phần tử cuối cùng như là prev.</dd>
  <dt>-Các hoạt động cơ bản trên Danh sách liên kết</dt>
  <dd>+Hoạt động chèn: thêm một phần tử vào đầu danh sách liên kết.</dd>
  <dd>+Hoạt động xóa (phần tử đầu): xóa một phần tử tại đầu danh sách liên kết.</dd>
  <dd>+Hiển thị: hiển thị toàn bộ danh sách.</dd>
  <dd>+Hoạt động tìm kiếm: tìm kiếm phần tử bởi sử dụng khóa (key) đã cung cấp.</dd>
  <dd>+Hoạt động xóa (bởi sử dụng khóa): xóa một phần tử bởi sử dụng khóa (key) đã cung cấp.</dd>
  <dt>-Danh sách liên kết đôi (Doubly Linked List) : hoạt động duyệt qua các nút có thể được thực hiện theo hai chiều: về trước và về sau một cách dễ dàng khi so sánh với Danh sách liên kết đơn. </dt>
  <dt>-Các hoạt động cơ bản trên Danh sách liên kết đôi</dt>
  <dd>+Hoạt động chèn: thêm một phần tử vào vị trí đầu của Danh sách liên kết.</dd>
  <dd>+Hoạt động xóa: xóa một phần tử tại vị trí đầu của Danh sách liên kết.</dd>
  <dd>+Hoạt động chèn vào cuối: thêm một phần tử vào vị trí cuối của Danh sách liên kết.</dd>
  <dd>+Hoạt động xóa phần tử cuối: xóa một phần tử tại vị trí cuối của Danh sách liên kết.</dd>
  <dd>+Hoạt động chèn vào sau: thêm một phần tử vào sau một phần tử của Danh sách liên kết.</dd>
  <dd>+Hoạt động xóa (bởi key): xóa một phần tử từ Danh sách liên kết bởi sử dụng khóa đã cung cấp.</dd>
  <dd>+Hiển thị danh sách về phía trước: hiển thị toàn bộ Danh sách liên kết theo chiều về phía trước.</dd>
  <dd>+Hiển thị danh sách về phía sau: hiển thị toàn bộ Danh sách liên kết theo chiều về phía sau.</dd>
  <dt>-Danh sách liên kết vòng (Circular Linked List) là phần tử đầu tiên trỏ tới phần tử cuối cùng và phần tử cuối cùng trỏ tới phần tử đầu tiên</dt>
  <dt>-Các hoạt động cơ bản trên Danh sách liên kết vòng</dt>
  <dd>+Hoạt động chèn: chèn một phần tử vào vị trí bắt đầu của Danh sách liên kết vòng.</dd>
  <dd>+Hoạt động xóa: xóa một phần tử của Danh sách liên kết vòng.</dd>
  <dd>+Hiển thị: hiển thị toàn bộ Danh sách liên kết vòng.</dd>
</dl>
***<br>
Ngày 02/02/2021<br>
Bài 7 - Reflection
<dl>SOLID là gì
<dt>-S : Single responsibility priciple</dt>
  <dd>+ý nghĩa là một class chỉ nên giữ một trách nhiệm duy nhất. Một class có quá nhiều chức năng sẽ trở nên cồng kềnh và trở nên khó đọc, khó maintain</dd>
  <dt>-O :Open/Closed principle</dt>
  <dd>+Không được sửa đổi một Class có sẵn, nhưng có thể mở rộng bằng kế thừa.</dd>
  <dt>-L :Liskov substitution principle</dt>
  <dd>+Các đối tượng (instance) kiểu class con có thể thay thế các đối tượng kiểu class cha mà không gây ra lỗi.</dd>
  <dt>-I :Interface segregation principle</dt>
  <dd>+Thay vì dùng 1 interface lớn, ta nên tách thành nhiều interface nhỏ, với nhiều mục đích cụ thể.</dd>
  <dt>-D :Dependency inversion principle</dt>
  <dd>+Các module cấp cao không nên phụ thuộc vào các modules cấp thấp. Cả 2 nên phụ thuộc vào abstraction.</dd>
  <dd>+Interface (abstraction) không nên phụ thuộc vào chi tiết, mà ngược lại (Các class giao tiếp với nhau thông qua interface (abstraction), không phải thông qua implementation.)</dd>
</dl><br>
<dl>
  <dt>-Các cách thực hành clean code</dt>
  <dd>+Sử dụng tên biến có ý nghĩa và dễ hiểu</dd>
  <dd>+Sử dụng cùng từ vựng cho cùng một loại biến</dd>
  <dd>+Đặt tên sao cho dễ tìm kiếm</dd>
  <dd>+Tránh lồng (nesting) quá nhiều và nên return sớm</dd>
  <dd>+Tránh hack não người đọc</dd>
  <dd>+Đừng thêm những nội dung không cần thiết</dd>
  <dd>+Sử dụng đối số mặc định thay vì phải kiểm tra bằng biểu thức điều kiện</dd>
  <dd>+Đối số của hàm (ít hơn hoặc bằng 2 là lý tưởng)</dd>
  <dd>+Hàm chỉ thực hiện một chức năng</dd>
  <dd>+Tên hàm nên thể hiện chức năng của hàm</dd>
  <dd>+Hàm chỉ nên có độ trừu tượng một cấp</dd>
  <dd>+Đừng sử dụng cờ như là một đối số của hàm</dd>
  <dd>+Đừng viết hàm global</dd>
  <dd>+Đừng sử dụng Singleton pattern</dd>
  <dd>+Đóng gói điều kiện</dd>
  <dd>+Tránh điều kiện phủ định</dd>
  <dd>+Xóa dead code</dd>
  <dd>+Sử dụng đối tượng đóng gói</dd>
  <dd>+Ưu tiên thành phần hơn kế thừa</dd>
  <dd>+Tránh viết fluent interfaces</dd>
  <dd>+Tuân thủ SOLID</dd>
  <dd>+Nguyên lý phân tách interface</dd>
  <dl>
***<br>
Ngày 01/02/2021<br>
Bài 6 - Reflection
<dl>Abstract class và class thường
  <dt>Giống nhau:</dt>
  <dd>-Đều là class</dd>
  <dd>-Có thể chứa thuộc tính, phương thức</dd>
  <dt>Khác nhau:</dt>
  <dd>-Abstract class có tính trừu tượng rất cao, không thể tạo được các đối tượng của lớp đó.</dd>
  <dd>-Phương thức được khai báo nhưng không có phần thân,ngoài ra nó còn có thể có thuộc tính và phương thức bình thường</dd>
  <dd>-Lớp bình thường kế thừa lớp abstract thì phải triển khai tất cả phương thức abstract</dd>
</dl>
<dl>Interface
<dt>là một chức năng mà bạn có thể thêm và bất kì class nào. Từ chức năng ở đây không đồng nghĩa với phương thức (hoặc hàm). Interface có thể bao gồm nhiều hàm/phương thức và tất cả chúng cùng phục vụ cho một chức năng.</dt>
  <dd>-Một class có thể thực hiện nhiều interface</dd>
  <dd>-Interface có thẻ kế thừa lẫn nhau</dd>
</dl>
###
***<br>
Ngày 29/01/2021<br>
Bài 5 - Reflection <br>
<dl>-<strong>Từ khóa final</strong>
  <dt>-Final là không cho phép phương thức đó bị ghi đè, nghĩa là chỉ cần ở lớp cha có từ khóa final là lớp đó sẽ không được kế thừa và ghi đè.</dt>
    <dd>class ConNguoi<br>
{
    private $soChan = 2;<br>

   final public function getSoChan()<br>
    {
        return $this->soChan;<br>
    }
}
<br>
//Sai vì không thể override lại final phương thức
class NguoiLon extends ConNguoi<br>
{<br>
    public function getSoChan()
    {<br>

    }
}<br>
//Fatal error: Cannot override final method ConNguoi::getSoChan()<dd>
</dl><br>
<dl><strong>Sự khác nhau giữa Overried và Overload</strong>
<dt>Override</dt>
  <dd>-Thay đổi hành vi hiện tại của phương thức.</dd>
  <dd>-Thể hiện tính đa hình tại run time.</dd>
  <dd>-Danh sách tham số phải giống nhau.</dd>
  <dd>-Phương thức ghi đè ở lớp con phải có quyền truy cập bằng hoặc lớn hơn phương thức được ghi đè ở lớp cha.</dd>
  <dd>-Kiểu trả về bắt buộc phải giống nhau.</dd>
  <dd>-Xảy ra giữa 2 class có quan hệ kế thừa</dd>
  <dt>Overload</dt>
  <dd>-Thêm hoặc mở rộng cho hành vi của phương thức.</dd>
  <dd>-Thể hiện tính đa hình tại compile time.</dd>
  <dd>-Danh sách tham số có thể khác nhau.</dd>
  <dd>-Các phương thức nạp chồng có thể có quyền truy cập khác nhau.</dd>
  <dd>-Kiểu trả về có thể khác nhau.</dd>
  <dd>-Xảy ra trong phạm vi cùng 1 class.</dd>
</dl>
<dl><strong>Constructor</strong>
  <dt>+là một phương thức đặc biệt, được thực thi ngay khi tạo ra đối tượng. Nó thường được sử dụng để khởi tạo các chức năng như gán thuộc tính với giá trị hay tạo ra các đối tượng khác từ đối tượng vừa tạo.</dt>
  <dd>VD: class demo<br>
{
    function __construct()<br>
    {
    }<br>
}</dd>
  <dt>-PHP không cho phép nhiều construct trong 1 class.</dt>
  <dt>-Khi nào thì lớp cha không cho phép lớp con kế thừa các thuộc tính và phương thức.</dt>
  <dd>+Khi lớp cha khai báo mức độ truy xuất là private</dd>
</dl>
###
***<br>
Ngày 28/01/2021 <br>
Bài 4 - Reflection<br>
<dl>
    <dt>-Namespace (tên miền không gian) là một hình thức để đóng gói các hạng mục có liên quan lại với nhau</dt>
    <dt>-Trong PHP, namespace được thiết kế để giải quyết 2 vấn đề mà các tác giả của các thư viện và ứng dụng thường gặp phải khi cố gắng tạo ra các đối tượng hoặc hàm có thể tái sử dụng được.</dt>
    <dd>+Các tên gọi bị trùng nhau giữa những lớp/hàm được tạo ra, so với các lớp/hàm có sẵn của PHP, hoặc các lớp/hàm do một người khác viết.</dd>
    <dd>+Khả năng để rút ngắn tên gọi thông qua việc đặt các bí danh (alias) nhằm giữ cho mã nguồn ngắn gọn</dd>
    </dl><br>
    <dl>PHP cũng là một ngôn ngữ lập trình nên nó cũng có cung cấp các thư viện xử lý JSON giúp lập trình viên giải quyết nó dễ dàng. Chúng ta có hai hàm đó là hàm json_decode và json_encode:
    <dt>json_decode: Hàm này mục đích chuyển một chuỗi JSON sang dạng mảng hoặc object,hàm này có cú pháp như sau: json_decode($json_string, $assoc)</dt>
    <dd>$json_string: là chuỗi JSON</dd>
    <dd>$assoc có hai giá trị true / false. Nếu true thì kết quả nó trả về là dạng  array, ngược lại nếu false thì kết quả trả về dạng object. Mặc định là false.</dd>
    <dt>json_encode: Hàm sẽ chuyển một mảng trong PHP hoặc object trong PHP thành chuỗi JSON.</dt>
    </dl>
    <br>
   <dl>-Cách dùng Composer : Autoload (Tránh cho việc phải dùng nhiều lần câu lệnh include hay require trong một tập kỹ thuật clean code)
    <dt>VD:require __DIR__ . '/vendor/autoload.php';</dt>
    <dd>{<br>
    "autoload": {<br>
        "psr-4": {"Acme\\": "src/"}<br>
    }<br>
}</dd>
</dl>
    
***
Ngày 27/01/2021<br>
Bài 3 – Reflection<br>
<dl>
-OOP xoay quanh khái niệm Lớp – class. Lớp là bản thiết kế hay bản mẫu\khuôn mẫu được sử dụng để tạo các đối tượng.<br>
<dt>+Các từ khoá public, protected và private còn được gọi là access modifier, tức là các từ khoá dùng để thay đổi mức độ truy cập của các thành phần.</dt>
<dd>Public có thể truy cập tới các phương thức và thuộc tính ở bất cứ đâu, dù trong nộ bộ của lớp hay ở lớp con hay cả bên ngoài lớp đều được</dd>
<dd>Private là thành phần chỉ dành riêng cho nội bộ của lớp, nghĩa là ta không thể truy xuất tới thành phần private ở lớp con hoặc ở bên ngoài lớp.</dd>
<dd>Mức truy cập protected chỉ cho phép truy xuất nội bộ trong lớp đó và lớp kế thừa, riêng ở bên ngoài lớp sẽ không truy xuất được</dd>
<dd>VD:</dd>
<dd>class Foo {<br>
    public $name;<br>
    private $age;<br>
    protected $address;<br>
}
</dd>
</dl>
<dl>Khi sử dụng từ khoá static với các thành phần của một lớp thì chúng có thể được truy cập thông qua tên của lớp mà không cần khởi tạo đối tượng. Một thuộc tính static thì không thể được truy cập thông qua một đối tượng của lớp đó, nhưng một phương thức static thì có thể được gọi thông qua một đối tượng của lớp.
<dt>VD:</dt>
<dd>class Foo<br>
{<br>
    public static $my_static = 'foo';<br>

public function staticValue() {<br>
return self::$my_static;<br>
    } }
</dd>
</dl>
