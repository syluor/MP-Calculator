# ��׼C++��ѧ����������

### ���򹲼�277�д��룬�����̡������Ĵ�������������
* �ҵ���ϵ��ʽ��
* QQ��13387073000
* Email��lhjok@live.cn
* ���͵�ַ��[�����Ĳ���](http://gogae.org/)

### ����ʵ�ֵĹ�����������
�ó���֧�����������㣬���ޱ���ʽ���ȣ�֧�֣�2560λ�����������㡢��ģ���㡢�˷����㡢���������ʵ�ù��ܡ�

֧�����������㣨�������� '^'Ϊ�˷������ . '%'Ϊ��ģ����� ��

`10-3*(2/1-(6*2+(21+3/5)*8/3)*-2)+8*2^2%3`

֧�ֺ���������㣨�������� "A=ABS" . "S=SQRT" . "P=PI"��'P'��ֱ����Ϊ���֣���

`10*(2/1-(6*2+(21.5A+3/5)-8*P/3)*23.5S)+8*2^2%3`

������Ӧ��Ƿ�����Ƿ�Ϊ��д����

A=�� ABS ����ֵ �� S=�� SQRT ƽ���� �� P=�� PI Բ���� ��

### ����ʹ����GMP��������⣺
GMP��һ����Դ�����⾫������⣬Ҳ��GNU��Ŀ��һ���֣�����Ŀ���ǳ�Ϊ���Ĵ�������⡣

### ��װMinGW-MSYS����������
1����װMinGW�����׼�����ֱ�Ӱ�װQT�����ṩ����������[QT-MinGW](http://www.qt.io/)��

2����װMSYS����������ֱ�����а�װ[MSYS](http://www.mingw.org/)��ִ���ļ����ɣ�

### ����GMP���ļ���
1������[GMP](https://gmplib.org/)���ļ��������ѹ��C�̸�Ŀ¼�£�

2���༭MSYS�����ļ���`C:/msys/1.0/etc/fstab.sample`

`C:/gmp`

3������MSYS���뻷����

`cd /c/gmp`

4������ִ���������

`./configure --enable-cxx`

`make`

`make check`

`make install`

5������GCC����������

`C_INCLUDEDE_PATH= C:\msys\1.0\local\include`

`CPLUS_INCLUDE_PATH= C:\msys\1.0\local\include`

`LIBRARY_PATH= C:\msys\1.0\local\lib`

### ��Դ����GCC���뻷�������ɿ�ִ���ļ���
1���½�һ��ͼ��("icon.rc")�ļ���
    
`1 ICON "ICON.ico"`
    
2��ʹ��"windres"��������.rc�ļ������Ŀ���ļ���
    
`windres icon.rc icon.o`
    
3��������ͼ��Ŀ�ִ�г���
    
`g++ -Wall -o Calculator -static Calculator.cpp icon.o -lgmpxx -lgmp`

4��ע��GMP������������Ѿ�������ˣ�����Ȥ��ͬѧ����ֱ��ʹ�ã��Ѿ����ϣ���