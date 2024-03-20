class Solution {
public:
    // Function to calculate combination "n choose r"
    long long nCr(int numRows, int r) {
        long long res = 1; // Initialize the result variable to 1
        for (int i = 0; i < r; i++) { // Loop to calculate factorial terms in nCr formula
            res = res * (numRows - i); // Calculate numerator: (numRows) * (numRows - 1) * ... * (numRows - r + 1)
            res = res / (i + 1); // Calculate denominator: (r) * (r - 1) * ... * 1
        }
        return res; // Return the result of nCr
    }

    // Function to generate Pascal's triangle up to numRows rows
    vector<vector<int>> generate(int numRows) {
        vector<vector<int>> triangle; // Initialize the 2D vector to hold the triangle
        for (int i = 0; i < numRows; i++) { // Loop to iterate through each row of the triangle
            vector<int> row; // Initialize a vector to hold the current row
            for (int j = 0; j <= i; j++) { // Loop to iterate through each element in the current row
                row.push_back(nCr(i, j)); // Add the value of combination "i choose j" to the current row
            }
            triangle.push_back(row); // Add the current row to the triangle
        }
        return triangle; // Return the generated Pascal's triangle
    }
};
