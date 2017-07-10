
# **Java**

''' 
package kr.ac.hufs;

public class HelloJava {

	public static void main(String[] args) {
		System.out.print("헬로 자바");
		/*ln은 줄바꿈*/
		System.out.println("헬로 자바2");
		showMsg("헬로 자바");
	}

	public static void showMsg(String msg) {
		/*msg라는 함수로 지정*/
		System.out.println(msg);
	}
}
'''


'''
	package kr.ac.hufs;

public class ClassTest {

	public static void main(String[] args) {
	A hufs = new A();
	hufs.m1();
	hufs.showMsgA();
	hufs.m2();
	hufs.showMsgA();

	}

}

class A{
	/*int는 정수함수를 정의 */
	int a = 100;
	/*문자를 정의해서 입력*/
	String str = "한국외국어대학교";
	
	A(){
		System.out.println("A() 생성자 호출");
	}
	
	public void showMsgA() {
	}

	void m1() {
		System.out.println("m1() 생성자 호출");
	}
	
	void m2() {
		a = a+1;
		System.out.println("a = " + a);
	}
}
'''
package kr.ac.hufs;

public class ClassTest2 {

	public static void main(String[] args) {
		hufs hufs = new hufs();
		hufs.setName("아이폰");
		hufs.showMsgName();/*showMsgName()은 출력하라는 명령어*/
	}
}

class hufs {
	int grade = 0;
	String name = "";
	
	hufs(){
		System.out.println("한국외국어대학교 전산망 입력입니다.");
	}

	void setName(String _name) {
		name= _name;
	}
	
	String getName() {
		return name;
	}
	
	void showMsgName() {
		System.out.println(name);
	}
	/*showMsgName()하고 결과값은 같다. 직방으로가냐 돌아서 가냐의 차이*/
	void showMsgName2() {
		String hufsName = getName();
		System.out.println(hufsName);
	}
}

'''

'''
package kr.ac.hufs;

public class ClassTest3 {

	public static void main(String[] args) {
		hufs2 hufs2 = new hufs2();
		hufs2.setName("플랭클린");
		hufs2.setGrade(4);
		hufs2.showMsgAll();

		A a = new A();
		a.m2();
	}
}


class hufs2 {
	int grade = 0;
	String name = "";
	
	hufs2(){
		System.out.println("한국외국어대학교 전산망 입력입니다.");
	}

	void setName(String _name) {
		name= _name;
	}
	void setGrade(int _grade) {
		grade= _grade;
	}
	
	String getName() {
		return name;
	}
	int getGrade() {
		return grade;
	}
	
	void showMsgAll() {
		System.out.println("이름: " + getName());
		System.out.println("학년: " + getGrade());
		
	}
	
	void showMsgName() {
		System.out.println(name);
	}
	/*showMsgName()하고 결과값은 같다. 직방으로가냐 돌아서 가냐의 차이*/
	void showMsgName2() {
		String hufsName = getName();
		System.out.println(hufsName);
	}
}

'''

'''
package kr.ac.hufs;

public class ClassTest4 {

	public static void main(String[] args) {
		hufs3 hufs3 = new hufs3();
		hufs3.setNameNsetGrade("플랭클린", 4);
	}
}



class hufs3 {
	int grade = 0;
	String name = "";


	/*N을 넣어 여러가지를 한번에 입력가능하다*/
	void setNameNsetGrade(String _name, int _grade) {
		name= _name;
		grade= _grade;
	}
	/*return은 한번에 하나씩 밖에 못한다.*/
	String getName() {
		return name;
	}
	int getGrade() {
		return grade;
	}	
}
	
'''

'''
package kr.ac.hufs;

public class StaticTest {

	public static void main(String[] args) {
		StaticTest st = new StaticTest();
		st.showMsg("한국외국어대학교");
		showMsg2("한국외국어대학교");
	}


	void showMsg(String _msg) {
		System.out.println(_msg);
	}
	static void showMsg2(String _msg) {
		System.out.println(_msg);

	}
}
'''

'''
package kr.ac.hufs;

public class Prac {

	public static void main(String[] args) {
		Aoa aoa = new Aoa();
		aoa.setName("설현");
		aoa.setBrt(950103);
		aoa.setAge(23);
		aoa.setEnt("FNC Entertainment");
		aoa.setAct("AOA 맴버로 활동하다가 단독 CF로 유명 스타로 오름");
		aoa.setEct("지코와 연애중");
		aoa.showMsgAll();
	}
}


class Aoa {

	
	Aoa(){
		System.out.println();
	}

	
	int brt = 0;
	int age = 0;
	String name = "";
	String ent = "";
	String act = "";
	String ect = "";


	void setName(String _name) {
		name= _name;
	}
	void setEnt(String _ent) {
		ent= _ent;
	}
	void setAct(String _act) {
		act= _act;
	}
	void setEct(String _ect) {
		ect= _ect;
	}
	void setBrt(int _brt) {
		brt= _brt;
	}
	void setAge(int _age) {
		age= _age;
	}


	int getBrt() {
		return brt;
	}
	int getAge() {
		return age;
	}
	String getName() {
		return name;
	}
	String getEnt() {
		return ent;
	}
	String getAct() {
		return act;
	}
	String getEct() {
		return ect;
	}


	void showMsgAll() {
		System.out.println("이름: " + getName());
		System.out.println("생년월일: " + getBrt());
		System.out.println("소속사: " + getEnt());
		System.out.println("활동내역: " + getAct());
		System.out.println("기타: " + getEct());
		System.out.println("나이: " + getAge());
	}

}	
'''
