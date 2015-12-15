# odd_sum-method
def odd_sum(*numbers)
    odd_numbs = Proc.new { |numbers| numbers.odd? }
    add = numbers.select(&odd_numbs)
    add.inject(:+)
end
