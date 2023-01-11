# git-repository
https://github.com/github/codespaces-blank.git

 import java.util.*;
 public class Solver
 {
    private ArrayList<item> menu;
    private ArrayList<String[]>solutions;

     public static class item
     {
         public String name;
         public int price;

         public Item (String name, int price)
         {
            this.name= name;
            this.price= price;
         }
     }
     price Solver (ArrayList<ITem> menu)
      {
        this.menu = menu;
      }
      public  ArrayList<String[]> solve (int budget)
         {
            solutions = new ArrayList<String[]<>();
            solve(new ArrayList<Item(),0,budget);
            return solutions;
         }
         private void solve (ArrayList<Item> items , int first, int budget)
         {
            if (budget ==0)
              {
                solutions.add(item.stream().map(e -> e.monday.toArray(String[]::new)));
              }
              else
              {
                for (int i = first; i<menu.size(); i++)
                {
                    items item = menu.get(i);
                    if(item.price<= budget)
                     {
                        items.add(item);
                        solve(items, i,budget-item.price);
                        items.remove(items.size()-1);
                     }
                }

              }
              public staticvoid main (String[] args)
              {
                ArrayList<Item> menu = new ArrayList<Item>();
                menu.add(new Item("monday",));
                menu.add(new Item("tuesday",));
                menu.add(new Item("thursday",));
                menu.add(new Item("friday",));
                menu.add(new Item("saturday",));
                menu.add(new Item("sunday",));
                solver solver = new Solver (menu);
                ArrayList<String[]> solution = solver.solve(550);
                for(int i =0; i<solutions.size();i++)
                System.out.println("solutions "+ (i+1)+":"+Arrays.toString(solutions.get(i)));
              }
         }
 }
