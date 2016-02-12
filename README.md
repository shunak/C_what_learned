# C


#include <stdio.h>

int main(int argc, const char * argv[]) {
  
    //読み込んだ正の整数値までカウントアップ
    
    /*
    
    int i,no;
    
    printf("正の整数を入力してください:");scanf("%d",&no);
    
    for (i=0; i<=no; i++)
        printf("%d",i);
        putchar('\n');
    
   */
    
    
    //読み込んだ整数の個数だけ*を連続表示(for文)
    
    /*
    int i,no;
    
    printf("正の整数を入力してください:");scanf("%d",&no);
    
    for (i=1; i<=no; i++) {
        putchar('*');
    }
    putchar('\n');
    
    */
    
    //指示された個数だけ整数を読み込んで合計値・平均値を表示（for文）
    /*
    
    int i;
    int sum=0;
    int num,tmp;
    
    printf("整数は何個ですか:");scanf("%d",&num);
    
    for (i=0; i<num; i++) {
        printf("No.%d:",i+1);scanf("%d",&tmp);
        sum+=tmp;
    }
    
    printf("合計値:%d\n",sum);
    printf("平均値:%.2f\n",(double)sum/num);
    
     */
    
    //演習4-12
    //List4-6をfor文を用いて書き換える
    
    /*
    
    int no;
    int sum;
    
    for (no=1; no<=5; no++) {
        sum+=no;
    }
    
    printf("1から5までを足した値は%dです。\n",sum);
     
     */
    
    //演習4-13
    //1234567890を繰り返し表示するプログラム
    
    /*
    int i,no;
    
    printf("整数を入力してください:");scanf("%d",&no);
    
    for (i=1; i<=no; i++) {
        printf("%d",i%10);
    }
    putchar('\n');
    
    //【超重要】%10で値の一の位を表示する。
    //【超重要】%10で値の一の位を表示する。
    //【超重要】%10で値の一の位を表示する。
    //【超重要】%10で値の一の位を表示する。
    //【超重要】%10で値の一の位を表示する。
    //【超重要】%10で値の一の位を表示する。
    //【超重要】%10で値の一の位を表示する。
     */
    
    
    
    //演習2-6
    
    //標準体重を実数で表示するプログラム
    
    /*
    int a;
    
    printf("身長を入力してください:");scanf("%d",&a);
    printf("標準体重は%.2fです。\n",(double)(a-100)*0.9);
    
    */
    
    
    
    
    //演習4-14
    /*
    
    
    int c,b,kizami;
    
    printf("身長に対する標準体重を示します。\n");
    printf("何cmから:");scanf("%d",&c);
    printf("何cmまで:");scanf("%d",&b);
    printf("何cmごと:");scanf("%d",&kizami);
    
    for (; c<=b; c+=kizami) {
        printf("%dcm %.2fkgです。\n",c,(double)(c-100)*0.9);
    }
    
    //for文の前処理部には何も必要ないので、省略。
    
    
    */
    
    
    ///多重ループ
    
    //演習4-15
    
    /*
    
    int i, j, k;
    
    printf(" |");
    
    for (i=1; i<=9; i++) {
        printf("  %d",i);
    }
    putchar('\n');
    
    for (k=1; k<=30; k++) {
        printf("-");
    }
    putchar('\n');
    
    for (i=1; i<=9; i++) {
        printf("%d|",i);
        for (j=1; j<=9; j++)
            printf("%3d",i*j); //%3d　続く実引数を少なくとも3桁で表示。
            putchar('\n');
    
    }
    
     */
    
    
    //List4-16
    //読み込んだ非負の整数値の個数だけ*を連続表示（好きなだけ繰り返す。）
    
    /*
    
    int cont;
    
    do{
        int num, i;
        
        do{
            printf("非負の整数を入力してください:");scanf("%d",&num);
            if(num<0)
                puts("\a負の数を入力しないでください。");
        } while (num<0);
        
        for (i=1; i<=num; i++)
            putchar('*');
        putchar('\n');
        
        printf("もう一度?【Yes・・・0/No・・・9】:");scanf("%d",&cont);
    } while(!cont);//論理否定演算子!a aが0であれば1,そうでなければ0(その型はint型)。
    
    //do文の中にdo文とfor文が入っている。
    
    */
    
    
    
    //List4-17 長方形
    
    /*
    
    int i, j;
    int width, height;
    
    puts("長方形を作りましょう。");
    printf("横幅:");scanf("%d",&width);
    printf("高さ:");scanf("%d",&height);
    
    for (i=1; i<=height; i++) {
        for (j=1; j<=width; j++)
            putchar('*');
        putchar('\n');
    }
    //プログラムは上から下に進むから、
    //for文の最初の変数にheightをとって、
    //iが高さがheightの範囲で変化しながら、
    //jのwidth、幅を増やすという構造をイメージ。
    
    //教科書的には、
    //height行の各列に、width個の*を並べると長方形が完成する。
    
     */
    
    
    //演習4-16
    
    /*
    
    int i, j;
    int sono1, sono2;
    
    puts("長方形を作りましょう。");
    printf("一辺（その1）:");scanf("%d",&sono1);
    printf("一辺（その2）:");scanf("%d",&sono2);
    
    for (i=1; i<=sono1; i++) {
        for (j=1; j<=sono2; j++)
            putchar('*');
        putchar('\n');
    }

     */
     
    //List4-18
    
    
    //直角三角形(左下が直角)を表示
    /*
    
    int i, j, ln;
    
    printf("何段ですか:");scanf("%d",&ln);
    
    for (i=1; i<=ln; i++) {
        for (j=1; j<=i; j++)
            putchar('*');
        putchar('\n');
    }

    */
    
    
    //List4-19
    
    /*
    
    int i, j, ln;
    
    printf("何段ですか:");scanf("%d",&ln);
    
    for (i=1; i<=ln; i++) {
        for (j=1; j<=ln-i; j++)
            putchar(' ');
        for (j=1; j<=i; j++)
        putchar('*');
        putchar('\n');
    }
    
    */

    
    //演習4-17
    
    //左上側が直角となる直角三角形
    
    /*
    
    int i, j, ln;
    
    printf("何段ですか:");scanf("%d",&ln);
    
    for (i=0; i<=ln; i++)
    {
        for (j=1; j<=ln-i; j++)
            putchar('*');
        putchar('\n');
    }

     */
    
    
    //右上側が直角となる三角形
    
    /*

    int i, j, ln;
    
    printf("何段ですか:");scanf("%d",&ln);
    
    for (i=0; i<=ln; i++)
    {
        for (j=0; j<=i-1; j++)
            putchar(' ');
        for (j=1; j<=ln-i; j++)
            putchar('*');
        putchar('\n');
    }
    
    */
    
    //演習4-18
    
    /*
    
    int i, j, lm;
    
    printf("ピラミッドを作りましょう。\n");
    
    printf("何段ですか:");scanf("%d",&lm);
    
    for (i=1; i<=lm; i++)
        
    {
        for (j=1; j<=lm-i; j++)
            putchar(' ');
        for (j=1; j<=2*i-1; j++)
            putchar('*');
        
        putchar('\n');
    }

    */
    
    
    
    
    
    //iが1の時 jを1から9まで増やしながら繰り返す
    //iが2の時 jを1から9まで増やしながら繰り返す
    //
    //
    return 0;

}

//for文
//for ~の間の意味。

//for（A;B;C）
//ループ本体
//Xcode的な構造解釈だと、
// for (<#initialization#>; <#condition#>; <#increment#>) {
//<#statements#>
//}

//つまり、for文はA,B,Cという3つの部分からなるが、
//その3つの部分A 初期値　B　条件　C　増分or減分
//で示される。

//教科書的には
//A　前処理
//Aが評価されるのは、繰り返しが行われる前の一度だけ。

//B 制御式
//繰り返しを行うかどうかの判定の為の制御式。
//この式を評価した値が非0であれば、ループ本体が実行される。
//このB部を省略した場合は、繰り返しの判定は常に非0となる。
//従って、break文などを使わない限り、無限ループとなってしまう。

//C 後始末
//C部はループ本体の最後に評価（実行）される。
//何も行うことがなければ、省略することができる。

//繰り返し文
//do文、while文、for文は、いずれもプログラムの流れを繰り返すためのもので、
//繰り返し文と呼ばれる。

//do文, while文, for文はいずれも自由に入れ子にすることができる。
//3重になっても,4重になってもよい。これらをまとめて多重ループという。







