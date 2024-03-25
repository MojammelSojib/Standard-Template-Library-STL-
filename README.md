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

13.Vector sort

#include<bits/stdc++.h>
using namespace std;
int main()
{
    vector<int>v1;
    v1.push_back(100);//v[0]
    v1.push_back(20);
    v1.push_back(300);
    v1.push_back(5);
    v1.push_back(10);

    cout<<"Before sort ";
    for(int i=0;i<v1.size();i++)
    {
        cout<<v1[i]<<" ";
    }
    cout<<endl;

    sort(v1.begin(),v1.end());
    cout<<"After sort ";
    for(int i=0;i<v1.size();i++)
    {
        cout<<v1[i]<<" ";
    }
    cout<<endl;

}

14.Reverse
#include<bits/stdc++.h>
using namespace std;
int main()
{
    vector<int>v1;
    v1.push_back(100);//v[0]
    v1.push_back(20);
    v1.push_back(300);
    v1.push_back(5);
    v1.push_back(10);

    cout<<"Before reverse ";
    for(int i=0;i<v1.size();i++)
    {
        cout<<v1[i]<<" ";
    }
    cout<<endl;

    reverse(v1.begin(),v1.end());
    cout<<"After reverse ";
    for(int i=0;i<v1.size();i++)
    {
        cout<<v1[i]<<" ";
    }
    cout<<endl;

}

14.Vector iterator
#include<bits/stdc++.h>
using namespace std;
int main()
{
    vector<int>v1;
    v1.push_back(100);//v[0]
    v1.push_back(20);
    v1.push_back(300);
    v1.push_back(5);

    vector<int>::iterator it;
    it=v1.begin()+3;
    cout<<*it<<endl;
}
all
#include<bits/stdc++.h>
using namespace std;
int main()
{
    vector<int>v1;
    v1.push_back(100);//v[0]
    v1.push_back(20);
    v1.push_back(300);
    v1.push_back(5);

    vector<int>::iterator it;

    for(it=v1.begin();it!=v1.end();it++)
    {
        cout<<*it<<endl;
    }
}
-----------
Part --  02
List
#include<bits/stdc++.h>
using namespace std;
int main()
{
    list<int>li;
    li.push_back(1);
    li.push_back(2);
    li.push_back(3);

    for(auto it:li){
        cout<<it<<" " ;
    }
    cout<<endl;

}

Try li.front & li.back li.size().liclear() li.empty()
--------------------
#include<bits/stdc++.h>
using namespace std;
int main()
{
    list<int>li;
    li.push_back(1);
    li.push_back(2);
    li.push_back(3);
    li.push_back(4);

    //li.clear();
    //li.pop_front();
    //li.pop_back();
    for(auto it:li){
        cout<<it<<" " ;
    }
    cout<<endl;
    cout<<li.size()<<endl;
    cout<<endl;

//if(li.empty())cout<<"Empty"<<endl;
  //  else cout<<"Not Empty";

}


Insert
-------------------
#include<bits/stdc++.h>
using namespace std;
int main()
{
    list<int>li;
    li.push_back(1);
    li.push_back(2);
    li.push_back(3);
    li.push_back(4);

    list<int>::iterator it;
    it=li.begin();
    advance(it,3);
    li.insert(it,4,5);

    for(auto it:li)
    {
        cout<<it<<" ";
    }
    cout<<endl;
}

-----------------
Specific vlue erase krbo
#include<bits/stdc++.h>
using namespace std;
int main()
{
    list<int>li={1,2,3,4,5,6};
    
    list<int>::iterator it;
    it=li.begin();
    advance(it,3);

    li.erase(it);
    for(auto it:li)
    {
        cout<<it<<" ";
    }
    cout<<endl;
}
----------------

Multipul value earse

#include<bits/stdc++.h>
using namespace std;
int main()
{
    list<int>li={1,2,3,4,5,6};

    list<int>::iterator it,it2;
    it=li.begin();
    it2=li.begin();
    advance(it2,3);

    li.erase(it,it2);

    for(auto it:li)
    {
        cout<<it<<" ";
    }
    cout<<endl;
}
-----------

Remove
#include<bits/stdc++.h>
using namespace std;
int main()
{
    list<int>li={1,2,3,4,5,6,3,3};
    li.remove(3);
    
    for(auto it:li)
    {
        cout<<it<<" ";
    }
    cout<<endl;
}
-------------------
reverse,sort,unique

#include<bits/stdc++.h>
using namespace std;
int main()
{
    list<int>li={1,2,3,4,5,6};
    //li.reverse()
    //li.sort()
    //li.unique();

    for(auto it:li)
    {
        cout<<it<<" ";
    }
    cout<<endl;
}
-------------------
swap

#include<bits/stdc++.h>
using namespace std;
int main()
{

    list<int>li={1,2,3,4,5,6};
    list<int>li2={3,4,5,6};

    li.swap(li2);

    for(auto it:li)
    cout<<it<<" ";
    cout<<endl;

    for(auto it:li2) cout<<it<<" ";
    cout<<endl;
}

-----------------------------
3.Deque(declar,pushback,size)

#include<bits/stdc++.h>
using namespace std;
int main()
{
    deque<int>dq;
    dq.push_back(1);
    dq.push_back(2);
    dq.push_back(3);

    for (int i = 0; i < dq.size(); ++i) {
        cout << dq[i] << " ";
    }
    cout << endl;

    int a=dq.size();
    cout<<a<<endl;

}




