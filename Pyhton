def calculate_glasgow_blatchford_score():
    # Input variables
    urea = float(input("Urea (mmol/L): "))
    hb = float(input("Hemoglobin (g/dL): "))
    systolic_bp = int(input("Systolic Blood Pressure (mmHg): "))
    heart_rate = int(input("Heart Rate (beats per minute): "))
    melena = input("Melena (Y/N): ").upper()

    # Scoring criteria weights
    urea_weight = 0.032
    hb_weight = 0.013
    systolic_bp_weight = 0.012
    heart_rate_weight = 0.139
    melena_weight = 0.679

    # Calculate GBS
    gbs = urea * urea_weight + hb * hb_weight + systolic_bp * systolic_bp_weight \
          + heart_rate * heart_rate_weight + (2 if melena == 'Y' else 0) * melena_weight

    return gbs

# Example usage
score = calculate_glasgow_blatchford_score()
print("Glasgow-Blatchford Bleeding Score:", score)
