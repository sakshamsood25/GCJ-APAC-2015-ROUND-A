//Saksham Sood
//GCJ-C
//Private
// Solution Begins
#include <cstdio>
#include <iostream>
#include <vector>
#include <list>
#include <queue>
#include <map>
#include <set>
#include <utility>
#include <functional> 
#include <string>
#include <algorithm>
#include <cmath>
#include <cstdlib>
#include <ctime>
//#include <deque>
using namespace std;

typedef long long ll;
typedef unsigned long long ull;
typedef pair<int,int> pii;
typedef map<int,int> mii;
typedef vector<int> vi;
typedef vector< vector<int> > vvi;
typedef vector<char> vc;
typedef vector<bool> vb;
typedef vector<string> vs;

#define rep(i,n) for(int i=0;i<n;i++)
#define forup(i,a,b) for(int i=a;i<=b;i++)
#define fordn(i,a,b) for(int i=a;i>=b;i--)
#define drep(i,n) for(i=0;i<n;i++)
#define dforup(i,a,b) for(i=a;i<=b;i++)
#define dfordn(i,a,b) for(i=a;i>=b;i--)
#define all(x) x.begin(),x.end()
#define permute(x) next_permutation(all(x))
#define ri(x) scanf("%d",&x)
#define rl(x) scanf("%lld",&x)
#define rd(x) scanf("%lf",&x);
#define rs(x) scanf(" %s",x);
#define pb push_back
#define mp make_pair
#define fi first
#define sc second
#define MOD 1000000007

int main()
{
	freopen("in.txt","r",stdin);
	freopen("out1.txt","w",stdout);
    int i,j,k,n,p,q;
    string s;
    int t,a[21][21];
    cin>>t;
    rep(z,t)
    {

        cin>>n>>s;
        rep(i,n)
        rep(j,n)
        cin>>a[i][j];
        
		cout<<"Case #"<<z+1<<":"<<endl;
            if(s == "right")
            {
                rep(i,n)
                {
                    p=n-1,q=n-2;
                    while(p!=0)
                    {
                        for(k=p;k>=0;k--)
                        {
                            if(a[i][k] != 0)
                            {
                                int c =a[i][p];
                                a[i][p]=a[i][k];
                                a[i][k]=c;
                                break;
                            }

                        }
                        if(k==0) {break;}
                        for(k=q;k>=0;k--)
                        {
                            if(a[i][k] != 0)
                            {
                                int temp =a[i][q];

                                a[i][q]=a[i][k];
                                a[i][k]=temp;
                                break;
                            }
                        }
                        if(a[i][p] == a[i][q])
                        {
                            a[i][p] = 2*a[i][p];
                            a[i][q] = 0;
                        }

                        p--;
                        q=p-1;
                    }
                }
            }
            else if(s == "left")
            {
                rep(i,n)
                {
                    p=0,q=1;
                    while(p!=n-1)
                    {
                        for(k=p;k<=n-1;k++)
                        {
                            if(a[i][k] != 0)
                            {
                                int temp =a[i][p];

                                a[i][p]=a[i][k];
                                a[i][k]=temp;
                                break;
                            }

                        }
                        if(k==n-1) {break;}
                        for(k=q;k<n;k++)
                        {
                            if(a[i][k] != 0)
                            {
                                int temp =a[i][q];

                                a[i][q]=a[i][k];
                                a[i][k]=temp;
                                break;
                            }
                        }
                        if(a[i][p] == a[i][q])
                        {
                            a[i][p] = 2*a[i][p];
                            a[i][q] = 0;
                        }

                        p++;
                        q=p+1;
                    }
                }

            }
            else if(s == "up")
            {
                rep(i,n)
                {
                    p=0,q=1;
                    while(p!=n-1)
                    {
                        for(k=p;k<=n-1;k++)
                        {
                            if(a[k][i] != 0)
                            {
                                int temp =a[p][i];

                                a[p][i]=a[k][i];
                                a[k][i]=temp;
                                break;
                            }

                        }
                        if(k==n-1) {break;}
                        for(k=q;k<n;k++)
                        {
                            if(a[k][i] != 0)
                            {
                                int temp =a[q][i];

                                a[q][i]=a[k][i];
                                a[k][i]=temp;
                                break;
                            }
                        }
                        if(a[p][i] == a[q][i])
                        {
                            a[p][i] = 2*a[p][i];
                            a[q][i] = 0;
                        }

                        p++;
                        q=p+1;
                    }
                }

            }
            else if(s == "down")
            {

                rep(i,n)
                {
                    p=n-1,q=n-2;
                    while(p!=0)
                    {
                        for(k=p;k>=0;k--)
                        {
                            if(a[k][i] != 0)
                            {
                                int temp =a[p][i];

                                a[p][i]=a[k][i];
                                a[k][i]=temp;
                                break;
                            }

                        }
                        if(k==0) {break;}
                        for(k=q;k>=0;k--)
                        {
                            if(a[k][i] != 0)
                            {
                                int temp =a[q][i];

                                a[q][i]=a[k][i];
                                a[k][i]=temp;
                                break;
                            }
                        }
                        if(a[p][i] == a[q][i])
                        {
                            a[p][i] = 2*a[p][i];
                            a[q][i] = 0;
                        }

                        p--;
                        q=p-1;
                    }
                }

            }
            rep(i,n)
            {
                rep(j,n)
                {
                    cout<<a[i][j]<<" ";
                }
                cout<<endl;
            }
    }
}
