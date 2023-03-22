#include<iostream>
#include<string>
using namespace std;
int main() {
	//string的三种构造函数
	string s1;
	char *str = "abc";
	string s2 = str;
	string s3(s2);        //string s3=s1;
	string s4(4, 'a');    //4个a
	cout << s1 << endl;
	cout << s2 << endl;
	cout << s3 << endl;
	cout << s4 << endl;
	string s5,s6,s7;
	s5.assign("hello world", 7);
	s6.assign(s5);
	s7.assign(10, 'w');
	cout << s5 << endl;
	cout << s6 << endl;
	cout << s7 << endl;
	//'+='==append()成员函数
	s2.append(s5, 2, 2);//s.append(str,pos,n),将str中下标从pos开始的n个字符添加到s末尾
	s5.append("hello", 4);//第一个参数为char*类型
	cout << s2 << endl;
	cout << s5 << endl;
}
https://github.com/yan-QAQ/STL_study/blob/main/string_%E6%9B%BF%E6%8D%A2%E6%9F%A5%E6%89%BE.png
