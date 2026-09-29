print("RECIPROCAL THEOREM")

# Original circuit
V1 = float(input("Enter voltage applied in original circuit (V): "))
R1 = float(input("Enter resistance R1 (ohms): "))
R2 = float(input("Enter resistance R2 (ohms): "))

# Current in the original circuit
I1 = V1 / (R1 + R2)

print("\nOriginal Circuit:")
print("Current I1 =", round(I1, 3), "A")

# Reciprocal circuit
V2 = float(input("\nEnter voltage applied in reciprocal circuit (V): "))

# Interchange source and response positions
I2 = V2 / (R1 + R2)

print("\nReciprocal Circuit:")
print("Current I2 =", round(I2, 3), "A")

# Check reciprocal condition
if abs(I1 / V1 - I2 / V2) < 0.0001:
    print("\nReciprocal Theorem is verified.")
else:
    print("\nReciprocal Theorem is not verified.")# reciprocal.py
reciprocal theorem
