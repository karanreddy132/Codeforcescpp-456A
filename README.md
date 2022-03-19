# Codeforcescpp-456A
#include <bits/stdc++.h>
 
using namespace std;
 
int main(){
  int n,ele1,ele2;
  cin >> n;
  vector<pair<int,int>> a;
  for(int i=0;i<n;i++){
    cin >> ele1 >> ele2;
    a.push_back(make_pair(ele1,ele2));
  }
  sort(a.begin(),a.end());
  for(int i=0;i<n-1;i++){
    if(a[i].first<a[i+1].first && a[i].second>a[i+1].second){
      cout << "Happy Alex";
      return 0;
    }
  }
  cout << "Poor Alex";
  return 0;
}
