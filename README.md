# Android Game Sederhana Lempar Coin

Nama	: Arkyana Usman Dwi B <br>
KLS	: TI.18.C.1 <br>
NIM	: 311810105 <br>
Mata Kuliah	: Pemograman Mobile <br>


<b>Tampilan di Menu Utama </b> <br><br>
![Menu Utama](https://raw.githubusercontent.com/arksm503/Android-LemparCoin/master/img/1.png)

<b>Penjelasan di Event OnClick</b>
``` Java
if (view==buttonToss) { 
```
Jika buttonToss ditekan maka tampilannya
``` Java
TextView tw=(TextView)findViewById(R.id.textView1);
ImageView iw=(ImageView)findViewById(R.id.imageView);
```
Identifkasikan dan cari ID.  tw dengan textView1, iw dengan imageView
``` Java
if (rand.nextDouble() < 0.5) {
    tw.setText("Kepala");
    iw.setImageResource(R.drawable.head);
```
Jika random next double kurang dari 0.5, maka akan muncul text “Kepala” dan gambar head <br><br>
![Head Button](https://raw.githubusercontent.com/arksm503/Android-LemparCoin/master/img/3.png)

``` Java
else {
    tw.setText("Cross");
    iw.setImageResource(R.drawable.tail);
```
selain itu, maka akan muncul text “Cross” dan gamber tail
``` Java
buttonToss.setVisibility(View.INVISIBLE);
buttonRepeat.setVisibility(View.VISIBLE);
buttonExit.setVisibility(View.VISIBLE);
```
buttonToss, disembunyikan, buttonRepeat dan buttonExit dimunculkan.<br><br>


![Tail Button](https://raw.githubusercontent.com/arksm503/Android-LemparCoin/master/img/4.png)
``` Java
else if (view==buttonRepeat) {
```
jika ditekan buttonRepeat maka akan muncul tampilan
``` Java
TextView tw=(TextView)findViewById(R.id.textView1);
ImageView iw=(ImageView)findViewById(R.id.imageView);
```
Identifkasikan dan cari ID.  tw dengan textView1, iw dengan imageView
``` Java
buttonToss.setVisibility(View.VISIBLE);
buttonRepeat.setVisibility(View.INVISIBLE);
buttonExit.setVisibility(View.INVISIBLE);
```
buttonToss, dimunculkan, buttonRepeat dan buttonExit disembunyikan. <br><br>

![Reapeat](https://raw.githubusercontent.com/arksm503/Android-LemparCoin/master/img/2.png)
``` Java
else if (view==buttonExit) {
```
jika klik buttonExit
``` Java
    this.finish();
```
keluar aplikasi.









