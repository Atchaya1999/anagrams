sing namespace std;
int main()
{   string A,B;
    int x;
    int count,y,z,sum;
    count=0;
    cin>>x;
  
    for(int i=0;i<x;i++)
    {
        cin>>A;
        cin>>B;
        y=A.length();
       z=B.length();
        for(int j=0;j<y;j++)
        {
           for(int k=0;k<z;k++)
           {
               if(A[j]==B[k])
               {   B[k]=0;
                   count++;
                   break;
               }
           }
        }
       
      sum=y+z-(2*count) ;
      cout<<sum<<endl;
      count=0;
     
    }
    return 0;
}
