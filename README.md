# Standard-Template-Library-STL-
#include<bits/stdc++.h>
using namespace std;
int main()
{
    int ar[100];
    vector<int>v;
    v.push_back(1);//v[0]
    v.push_back(22);//v[1]
    v.push_back(3);//v[2]
    v.push_back(4);//v[3]
    v.push_back(5);//v[4]v.push_back(1);//v[0]

    cout<<v[0]<<endl;
    cout<<v[1]<<endl;
    
      cout<<v.at(0)<<" ";//at bebohar kora hoy karon garbag vaule print kore na
    cout<<v.at(1)<<endl;

    cout<<v.size()<<" ";    // size print kora vector er(3)

      for(int i=0;i<v.size();i++)
   {
       cout<<v[i]<<" ";
   }                      //loop er modde vlue gula print kora dice


 cout<<v.front()<<endl;// 5.front function amra 1st value print kora nite pari
cout<<v.back()<<endl;//6.back function amra last value ta print krte pari


v.clear();
    cout<<v.size()<<endl;//7.clear kori sob kicu

if(v.empty()) cout<<"Empty"<<endl;
    else
        cout<<"Not Empty"<<endl;//8.empty ki na check kora

//9.pop_back last er ta delete kora dei
  v.pop_back();
    for(int i=0;i<v.size();i++)
   {
       cout<<v[i]<<" ";
   }        

//10.Kon value ke delete korbo
  v.erase(v.begin()+2,v.end());

     for(int i=0;i<v.size();i++)
   {
       cout<<v[i]<<" ";
   }    
}


11..Insert--cpp

#include<bits/stdc++.h>
using namespace std;
int main()
{
    vector<int>v;
    v.push_back(10);//v[0]
    v.push_back(20);//v[1]
    v.push_back(30);//v[2]
    v.push_back(40);//v[3]
    v.push_back(50);//v[4]v.push_back(1);//v[0]

   for(int i=0;i<v.size();i++)
   {
       cout<<v[i]<<" ";
   }
   cout<<endl;

   v.insert(v.begin()+2,3,1);

   for(int i=0;i<v.size();i++)
   {
       cout<<v[i]<<" ";
   }
}

12.swap
#include<bits/stdc++.h>
using namespace std;
int main()
{
    vector<int>v1;
    v1.push_back(10);//v[0]
    v1.push_back(20);//v[1]
    v1.push_back(30);//v[2]
    v1.push_back(40);//v[3]
    v1.push_back(50);//v[4]v.push_back(1);//v[0]

    vector<int>v2;
    v2.push_back(1);
    v2.push_back(2);
    v2.push_back(3);

    cout<<"Before swaping"<<endl;
    for(int i=0;i<v1.size();i++)
    {
        cout<<v1[i]<<" ";
    }
   cout<<endl;

       for(int i=0;i<v2.size();i++)
    {
        cout<<v2[i]<<" ";
    }
   cout<<endl;

   swap(v1,v2);
   cout<<"Ater swaping"<<endl;
    for(int i=0;i<v1.size();i++)
    {
        cout<<v1[i]<<" ";
    }
   cout<<endl;

       for(int i=0;i<v2.size();i++)
    {
        cout<<v2[i]<<" ";
    }
   cout<<endl;

}



