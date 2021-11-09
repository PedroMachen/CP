////////////////////////criba para encotrar primos menores a n
int countPrimes(int n) {
      bool arr[n+5];
      int cont = 0;
      for(int i=2; i<n; i++){
          arr[i] = true;
      }

      for(int i =2; i*i<n; i++){
          if(!arr[i]) continue;
          for(int j=(i+i); j<n; j+=i){
              arr[j] = false;
          }
      }

      for(int i=2; i<n; i++){
          if(arr[i])cont++;
      }

      return cont;
  }
/////////////////////////////////////////////// is prime?
bool is_prime(int n) {
    
    if (n == 1) {
        return false;
    }

    int i = 2;
   
    while (i*i <= n) {
        
        if (n % i == 0) {
            
            return false;
        }
        i += 1;
    }
   
    return true;
}
/////////////////////////////////////////////////////////// exp binaria

long long binpow(long long a, long long b, long long m) {
    a %= m;
    long long res = 1;
    while (b > 0) {
        if (b & 1)
            res = res * a % m;
        a = a * a % m;
        b >>= 1;
    }
    return res;
}

//////////////////////////////////////////////////////ncr

long ncr(int n, int r) {
        long ans = 1;
        for(int i = 0; i < r; i++) {
            ans *= n-i;
            ans /= i+1;
        }
        return ans;   
    }
    
 /////////////////////////////////////////////////// 
