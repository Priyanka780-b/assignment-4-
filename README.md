//Implement a function that finds the maximum element in an array using linear search.

public class MaxElementLinearSearch {

    // Function to find the maximum element in an array using linear search
    public static int findMax(int[] array) {
        if (array == null || array.length == 0) {
            throw new IllegalArgumentException("Array cannot be null or empty.");
        }

        int max = array[0]; // Assume the first element is the maximum

        for (int i = 1; i < array.length; i++) {
            if (array[i] > max) {
                max = array[i]; // Update max if a larger element is found
            }
        }

        return max;
    }

    public static void main(String[] args) {
        int[] numbers = {15, 42, 7, 29, 89, 63};
        int max = findMax(numbers);
        System.out.println("Maximum element is: " + max);
    }
}
