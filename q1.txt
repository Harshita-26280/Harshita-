public class HighestSalesDay {
    public static void main(String[] args) {
        // Sample sales data for each day (index represents the day, value represents sales)
        int[] sales = {150, 200, 250, 300, 400, 350, 500};
        
        // Variables to track the highest sales and corresponding day
        int maxSales = sales[0]; // Assume first day's sales is the highest initially
        int maxDay = 0; // Index of the highest sales day
        
        // Loop through the sales array to find the highest sales day
        for (int i = 1; i < sales.length; i++) {
            if (sales[i] > maxSales) { // If current day's sales is higher than maxSales
                maxSales = sales[i]; // Update maxSales
                maxDay = i; // Update maxDay
            }
        }
        
        // Display the result (Adding 1 to maxDay to represent day in human-friendly format)
        System.out.println("The highest sales were on day " + (maxDay + 1) + " with sales of " + maxSales);
    }
}
