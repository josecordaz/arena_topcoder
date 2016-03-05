package initialtarjet;

public class InitialTarjet {

    public static void main(String[] args) {
        InitialTarjet it = new InitialTarjet();
        System.out.println(
            it.canObtain(
                "AAABBAABB",
                "BAABAAABAABAABBBAAAAAABBAABBBBBBBABB"
            )
        );
    }   
    
    public String canObtain(String initial,String target){
        String res = "Impossible";
        if(!initial.equals(target)){
            if(target.contains(initial+"A")||target.contains(new StringBuilder(initial+"A").reverse().toString())){
                res = canObtain(initial+"A",target);
            }else{
                res = canObtain("B"+new StringBuilder(initial).reverse().toString(),target);
            }
        } else {
            res = "Possible";
        }
        return res;
    }
}
