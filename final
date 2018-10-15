#include <bits/stdc++.h>

using namespace std;

// Complete the nonDivisibleSubset function below.
int nonDivisibleSubset(int k, vector<int> S) {
int i,j,count=0;

    vector<int> a[k];
    for(i=0;i<S.size();++i)
        a[(S[i]%k)].push_back(S[i]);
    cout<<endl;
    for(i=0;i<k;++i)
        {for(j=0;j<a[i].size();++j)
            cout<<a[i][j]<<' ';
        cout<<endl;
        }
    cout<<endl;
    if(a[0].size()!=0)
        count++;
    for(i=1;i<=k/2;++i)
    {
        cout<<((a[i].size()>=a[k-i].size())? a[i].size():a[k-i].size())<<' ';
        count+=((a[i].size()>=a[k-i].size())? a[i].size():a[k-i].size());
        cout<<count<<endl;
    }
    cout<<endl;
    if(k%2==0)
        if(a[k/2].size())
                count=count-a[k/2].size()+1;
    return count;
}

int main()
{
  vector <int> s;
  int n,k,i,temp;
  cin>>n>>k;
  for(i=0;i<n;++i)
  {
    cin>>temp;
    s.push_back(temp);
  }
  cout<<nonDivisibleSubset(k,s);
  return 0;
}
