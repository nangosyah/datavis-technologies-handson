 <div>
    <p>The circumference of a sphere with radius {radius}m is {calculateCircumference(radius)}m.</p>
</div>


<script>
  const radius = 5;

  function calculateCircumference(radius) {
    const circumference = 2 * Math.PI * radius;
    return circumference.toFixed(2);
  }
</script>
