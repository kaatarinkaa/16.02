# #include <iostream>
#include <vector>
using namespace std;
int main()
{
	vector <int> sk{ 1, 2, 3, 1, 2 };

	if (sk[0] == 1) cout << "pirmaja vieta ir 1" << endl;
	if (sk[1] == 1) cout << "otraja vieta ir 1" << endl;
	if (sk[2] == 1) cout << "tresaja vieta ir 1" << endl;
	if (sk[3] == 1) cout << "ceturtaja vieta ir 1" << endl;
	if (sk[4] == 1) cout << "piektaja vieta ir 1" << endl;

	if (sk[0] == 4) cout << "pirmaja vieta ir 4" << endl;
	if (sk[1] == 4) cout << "otraja vieta ir 4" << endl;
	if (sk[2] == 4) cout << "tresaja vieta ir 4" << endl;
	if (sk[3] == 4) cout << "ceturtaja vieta ir 4" << endl;
	if (sk[4] == 4) cout << "piektaja vieta ir 4" << endl;

	//string atb, num;
	//vector <string> country {"USA", "UK", "China", "India", "Canada", "Australia"};
	//vector <string> code {"+1", "+44", "+86", "+91", "+1", "+61"};
	//cin >> atb;
	//if (code[0] == atb) { cout << country[0] <<" "<< atb << num << endl; }
	//if (code[1] == atb) { cout << country[1] << " " << atb << num << endl; }
	//if (code[2] == atb) { cout << country[2] << " " << atb << num << endl; }
	//if (code[3] == atb) { cout << country[3] << " " << atb << num << endl; }
	//if (code[4] == atb) { cout << country[4] << " " << atb << num << endl; }

	int atzime;
//vector atz{ 3,8,7,4 };
//vector name{ "Anna", "Antons","Vlads","Artemijs" };
//cout << "enter mark" << endl;
//cin >> atbild;
//if (atz[0] == atbild) { cout << name[0] << endl; }
//if (atz[1] == atbild) { cout << name[1] << endl; }
//if (atz[2] == atbild) { cout << name[2] << endl; }
//if (atz[3] == atbild) { cout << name[3] << endl; }
//else cout << "nav";
}


CREATE TABLE EMPLOYEE (
  Id INTEGER PRIMARY KEY,
  kurjera_v TEXT NOT NULL,
  kurjera_u TEXT NOT null,
  rajons TEXT NOT NULL,
  vecums INTEGER NOT NULL,
  dzimums text not null
  );
  INSERT INTO EMPLOYEE VALUES (1, 'Alla', 'Kotova', 'Riga',32, 'sieviete' );
  INSERT INTO EMPLOYEE VALUES (2, 'Vlads', 'Krastiņš', 'Riga',45, 'virietis');
  INSERT INTO EMPLOYEE VALUES (3, 'Grigorijs', 'Galds', 'ogres rajons',33, 'virietis' );
  INSERT INTO EMPLOYEE VALUES (4, 'Kira', 'Klimova', 'saulkrastu novads',56, 'sieviete');
  SELECT* FROM EMPLOYEE;
  SELECT* FROM EMPLOYEE;
  SELECT* FROM EMPLOYEE where vecums> 45;
  SELECT* FROM EMPLOYEE where rajons = 'Riga' and dzimums = 'virietis';
  SELECT avg (vecums)
  FROM EMPLOYEE;
  SELECT min (vecums)
  FROM EMPLOYEE;
CREATE TABLE EMPLOYEE (
emlpoye_ID INTEGER NOT NULL,
kurjera_v TEXT NOT NULL,
kurjera_u TEXT NOT NULL,
customer_ID INTEGER NOT NULL,
customer_name TEXT NOT NULL,
pilseta TEXT NOT NULL
);
-- insert
INSERT INTO EMPLOYEE VALUES (1, 'Thomas(Neo)', 'Anderson', 1, 'Jewelry Store', 'London');
INSERT INTO EMPLOYEE VALUES (1, 'Thomas(Neo)', 'Anderson', 2, 'Bakery', 'London');
INSERT INTO EMPLOYEE VALUES (1, 'Thomas(Neo)', 'Anderson', 3, 'Cafe', 'London');
INSERT INTO EMPLOYEE VALUES (1, 'Thomas(Neo)', 'Anderson', 4, 'Restaurant', 'London');
INSERT INTO EMPLOYEE VALUES (2, 'Agent', 'Smith', 1,'Jewelry Store', 'Cardiff');
INSERT INTO EMPLOYEE VALUES (2, 'Agent', 'Smith', 2,'Bakery', 'Cardiff');
INSERT INTO EMPLOYEE VALUES (2, 'Agent', 'Smith', 3,'Cafe', 'Cardiff');
INSERT INTO EMPLOYEE VALUES (2, 'Agent', 'Smith', 4,'Restaurant', 'Cardiff');
-- fetch
SELECT * FROM EMPLOYEE WHERE customer_name='Bakery';
SELECT * FROM EMPLOYEE WHERE emlpoye_ID=4 and kurjera_u='Anderson';
SELECT AVG(customer_ID) FROM EMPLOYEE;
SELECT MIN(customer_ID) FROM EMPLOYEE;
